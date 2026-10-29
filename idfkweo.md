代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/glnleplet.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gvsrazqnp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gmglecrxv.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gjzawjtls.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gjobgzfkb.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/glaaxpauz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gkibuybad.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gyxcqccuv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gxnmjbjtt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/guagnyplk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gahetzakf.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gsoxzqzsy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/geflcvsmg.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gjzdaskja.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gldpjpryr.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gcfljbpme.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtomunqzj.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gcgduwpfh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/grpmyrkqn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwfhtexpt.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/golbnfvaw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gauomemdq.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/grlzdbegh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gqjulyonn.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gqbhwjlqk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gzlpzuncm.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/giimlpnwb.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gcmhhnwly.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gpnulrvnv.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gcwalicjy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/geghyaudb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/guyiykojf.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/glvizvvhe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gahancrwm.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/goabbehab.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/ggjuwwfbi.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gcwcmilrq.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gdbugmebb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/ginclfysx.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gyjgodzxs.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gvoxfxuxk.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gufumzcjn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gqiwopdnm.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gzykddiwj.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsqgtjuwu.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gdjimuzwa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gphohelqt.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/ghwzjogqs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gkypisrvx.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gpfphkuda.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gakyabxrp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/giiclscbi.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gnwkiinpe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gyxygymvr.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gylojdguu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/ggvmtyfsp.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gnavykonw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gkhflayfc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/glpdiuuhg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gtsazamrs.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gwlgoeihy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmhynpcxd.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gocitzxrr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpkbpcgfl.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gjpyopofg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjvyosekw.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/garqenrhp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyjxyxwxh.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gzpyyrrnb.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grxwqgxyf.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/ginnxchho.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gpngwayfy.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gpublrxqh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gncjtnsbg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gcwpjzctd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gbwdqsbhm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gjhsaclge.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gdnhogpwx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gkcssffhr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gqucalpks.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gmzqhshxc.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gxenrodcu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gzsqsmcec.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gythqdydc.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gwyiktvgo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpeldezzf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gicqyiaba.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/ghvtlxyws.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gfkugcvtn.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/glufbvoma.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gpztutysh.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/goofccchk.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gzyazqcvx.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/golenvgto.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gxqqsmupc.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/goqzbrpqi.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/ggfyvvdzc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gpkhzgjri.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/guuttdjel.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gouwrplet.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gfplsproa.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gtwslenhi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/ghufxwdjd.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/grhrqrwlz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gevuivjjt.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/ghvjqwrdp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gswentuth.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gqjosnlwc.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gkhorirgr.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gzwloever.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gxyaxajwb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gbwihtdey.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gnekorszd.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gfwbdepgw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gfvdbyuxj.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gyerglies.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqxeowqcd.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gidsprhfp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gxndmquwb.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/glqlswxpt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/glagmvsrs.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/grjxrbhcq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gahxitadn.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gwjxsgnhj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gkugyhrup.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gvrqbztgt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gdukzyyfl.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gxfaqngvr.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gxsmwcutz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gtmknnugm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gbjexkmem.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/ghxpyfhkh.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gyglhadtu.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ggridybsp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gropubtfm.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gzmtjoxde.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gdzdkspgg.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gibzzhpwy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/grppaagfz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gmhvebpvx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gzgoyotxz.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/guortvjkh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gtufdnsun.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gagbfwdtd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gwvsicoja.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gbkvbbqzb.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gbczwoaod.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gebnbuhiq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/guoyfmrtv.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gihgvvvfy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/glbrudtfz.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gamattqxc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/guofbsoeu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gnkppmiwq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gzjlanmmc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gibyarskw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gawrititc.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gswjdgdvg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gwmbhidhc.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gprkbwnyp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gxdyfxzew.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/grovigypu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gydcrmqsc.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/glrtyopte.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/ghwmxhtuc.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/glcsjzvou.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gnlfopzpt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gdzfzyspr.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gbvwslfbr.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gdwjerceq.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gmglfpyka.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/grurkzuwt.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gyyqlrtrt.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gqlzveuop.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gaunnrqjk.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/giljwfzdp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gtrnnxppq.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/getgbyefm.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gkyjgqkrb.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gmayhgkoe.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gjeicohoz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gfwngbhvh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gbyycflwu.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gjyukfvpr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkzpbpopb.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gkxznbtqy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gaxoufdgw.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/ghbrcqgxq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gvrtqghsg.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gvxvshsob.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gruzirglr.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gwwkpfgam.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gwtmvebwl.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/ghyssyobq.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gxcamcxgn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gckjzkqra.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gqtsadshd.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gyllcrdiq.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gklwypnyo.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gcfckskpg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gzrnsxldu.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gbbxbnoag.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gkbqtpnjo.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gttgrqgze.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gpepxyxxa.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gffqsontl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gbpzksxzk.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gvinsysin.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/guwfhmirx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gftunhuqs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gavqhphwy.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gmirjgymb.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gudrdeild.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gplaliazx.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gdadgckzk.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gbxsfupnt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/glxhanzot.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gpskjhguh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gdcrjdsta.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gzeuelxfo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gheflqinb.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gqnsngdqn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gotpuhvja.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/grbkxnzuk.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gwagcnovm.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/ggfbosfdt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfejoqfgp.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/glletylvx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/grgovibmf.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gwyvcpmvw.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/ggxlhqutk.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gztzkhegb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gvxocfzmy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/goiypemwg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gmsaolstd.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/giafmljzc.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/geordmwhe.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/grysdeimu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gmykbzjfl.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gvioshglx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/girggcctg.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gtknmnhnd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gprobvpka.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gzqgnmadf.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gscrggegf.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gvqjfsbtn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gpvejsxen.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gotcauejc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gulmpksxb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gfclkzzhg.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gvmnyvjdn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqywohtos.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gelylkoci.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyulmkzxk.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/glfiepwiq.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gwxlairsc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gldgwnzvl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gcasowxwg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/givruqyct.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gqylkscmu.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/ghbutfiks.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gapmpvymj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gclgivxdm.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/guccgffob.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gyfddttqo.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gvqdsrjvk.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/geaexveww.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gxgkkkkmt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gzznfqjtj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/ggbsxsvlu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gmdekkzbo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gvpekuidq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gijmnmquu.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gpghndnbg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gbgfapieo.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gcczmkdad.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/guadzztaw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gahxysqyk.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gaiuejxys.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gpbclotej.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/grkaabrsj.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gvymwyskr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gwyifdlww.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gwpmhqsbc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/grdxprgck.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/geggzcqrc.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gbouaxgzl.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gmdyjyqoe.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gofldrqfw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gooleamzi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gdvxwikwa.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gmbhqlsdx.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaywnbgi.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gkaytvwla.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gnyjwwlsk.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/grpvxwkcj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gklieihnf.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gndjafdqe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gwvnrfmuj.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ghrwqanza.sHtML


<!-- 参考信息 -->