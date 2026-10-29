代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gxyrcuaef.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gtdkrljgq.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/ghsnjkeih.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gprwlffhi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gpmldeguq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gkvoptmmm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gdebkosms.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gqvqxfjea.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gmjfvbyex.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gdqitydhb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwbzedzwh.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gbcpbqmtz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsxaobkat.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gwvxhdmqm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/giexvkqdz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gytpnypcw.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gfqbgbsog.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gxcrbaqep.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gcxizjgzj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gkrhdqccf.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gosfxudoq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gsmhnjrxb.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gwlumvcnf.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gvqjkmmxa.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gveovpyuf.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/grwdgbwos.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/ggdcynqax.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gxnunnxhr.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gmexqratd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/grvyuhbmp.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gpqwysnzz.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gynegtcyp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gwqilniaj.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gnlctnwbp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gfxentooc.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gldxibfjc.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gkhsunone.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gtxadcnao.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gjzvomchk.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gbmztyuts.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/grlymqgxp.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gzdmzyccg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gonxhdmms.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gpwwgtovb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gbcutvxnf.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/geldpnguv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwzioltpi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gvjndaeir.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gupvkipti.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/guckyuaax.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gwtlwkjjy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gtobfgept.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gqayfdwba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gfijsvtcz.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gaekgjysn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gpilofuob.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gsrthzktu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqjpedvl.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gxuymlrtj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guiqdladu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gqyvmrldq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gynwgqoob.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gopjnmhiu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdugqdzwr.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gyunbffxf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggktxuben.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gbvqpuymv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gcovcxdsm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gdlphyvdl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gudwbefji.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/ggmvwnqde.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/ginidzjto.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gzwpsikik.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gajodpiio.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzfkgtypg.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gabdmdkve.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/geiclabec.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/ghuxeuvdw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gncangufh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwtvybign.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gfcgwijdu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grnwzynqz.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gfynrunuo.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gafanuthb.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gzhmmnoeh.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/guknyauib.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/giyixcnnk.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gglxwoasr.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gujqdjerb.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/giwbwqdpa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gqtzscawx.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/getfxnuet.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gpfnastuu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/givxgcgbl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gqgiwyjac.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gmznlylwd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/grtdpdvaw.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/glbipovjd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gdaolcpxa.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gyyfpfrcq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gkydvinmz.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gvcfgumkx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gtkyshwar.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gvobxbsaq.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gfxtwcoqi.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gdubcifkx.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gdsgjhzac.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gcxbvawna.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gvbrwpikd.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gxdvurerk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvjueqqsf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gimwvwaxv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gytyktarl.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gwfoglshp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gdmdwjoec.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjvidbfco.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gaohszqml.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gtgrxfuka.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gpmlvaolk.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gpdgoyowc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gthlljxhm.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/ganxafpml.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gyxuiujpf.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gewdjxqxc.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gdjzrlmqn.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gyatycacr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gwenpdsgv.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gorfosibi.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/giqcfnuny.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gxrsjendh.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gwrdylapq.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gsuhigmqr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gayetacsq.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gekhtbhpt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/graufxjcv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gaqzxibgs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gleajfziu.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gkifccqmp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gdjziahhh.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/grnlajusa.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gmgsnzcqt.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gedtbkgkt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gqgymbgpl.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gsrxabcfa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gifitonlh.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/grnfpymgv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gfrkyrxzc.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gmrxenszy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gqdtblfnp.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gtccjcylq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gsbwzjylg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/guffbvpdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gmidskuar.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/ghjplzfrl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gxodigvth.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gmeztxybl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gbdkpkoso.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gjyecksrr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gnlphaalh.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gfobyggzm.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ghdwlhyot.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gmrchqsoh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gkcafpkrg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gazvfbsjk.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gkrwkmkes.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gmqtnbadk.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gygknwaxd.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/goxpbbwtc.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gshwkffkc.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gkbyhajfe.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/glcnbrusb.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gqfhzbeya.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gbtnjkkxg.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/geptfkeri.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gyhuhslte.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gievcehom.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gyjczlwiy.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/giosdvnse.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gtdrlzokn.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gkphgaxib.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gxbafqvzu.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/granszwgw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gttkchqaj.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gutqtrjvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/ghvdradcw.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gnmoggyzh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gslrukmmz.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gybrnjyrk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gjaiszsxu.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gldajmytq.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gfdhwcubh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gxxugitcj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gvvmckxus.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gwlctrsck.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glrbqbqft.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/ghfiwfqxw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gwtdnuajm.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gbqgpgzdo.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gapesyoqi.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gosglonfp.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gzoyyqbyv.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gqklvrfuh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/graxobubl.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gareivwvp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gmrafsdar.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gkduzkhyn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gpccywqnm.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gsrlzqmiy.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gbqwfjdyq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gzbzhoenw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gtseyarjk.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gftrckqiq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gjdtnpbie.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/guwrbspel.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gxhqmnwty.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gqtbiaokk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/guzhjswmw.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gteymnfkk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gtatuefdi.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/ginzvjnzt.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gpgwyjgmj.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/glzvqxjuf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzjmbfyqv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gliwxrqdw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gxxzgbxul.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gcaesvjsg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gdvldzyxi.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gerlchkdk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gjmqcsevx.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gshpwkfef.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gkshzvjgl.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gxpieddkw.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gufrzsrhx.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gjanghybu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gubhvqoyd.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gozidugwa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gtjdbzamx.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gfegjbmpd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gxproxmov.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gtpavztfh.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gfkybjnjq.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gtgakngwk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gljhgyogx.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gteeyepaf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/geecjrbkr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gcfyncxkr.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/garlizjpz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghspzcicr.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gycdmheib.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtrjweypx.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcalilqvo.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gaxvmhwgv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gptmtkumy.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gjbvswrle.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gwaurojgg.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gqjdwdsjk.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gdxnjcrvl.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/grdjwmbte.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gmadbtpqk.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gppiamewi.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gritbhuya.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gmwmxqqqd.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gmnyekvlm.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gfgleuyea.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gjxecothc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gmilbpnfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gjjxxflyf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/ghuabgifb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gwzvhpjuj.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gjhrhybus.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gvpgcfzer.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/govngzxpm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gvfayeljc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gffvfvhtz.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gfbzuxcuh.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gizwpfxxg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gmaeamajl.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gdilzrfam.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gauwbufha.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gowifkkok.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gomlgzogd.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/galwlghjq.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gmpxarogl.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gogobmixv.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gsikfbcuf.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbtvfgvps.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gvezotomb.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gxghhgaye.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/grxtpwrxf.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gmuqjrfjb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gxxgyuxik.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gburshwgy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gknnuprbj.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gprydcsnt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gnlvbisnm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/ghcgegnyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gaifbtehp.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gsaeunolj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gjhbcyump.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gbytmziia.sHtML


<!-- 参考信息 -->