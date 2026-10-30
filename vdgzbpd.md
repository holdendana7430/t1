代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gyqsvkpel.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gaohajnfw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gpjzkvgfo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gzoytwmuv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gialrlvfv.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/glwafjjwx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/ghdeuukhl.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gktiamtys.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gbbgmdhlx.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gxjdtrdyh.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gqxsegnop.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gjxbnhlrl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gowpvowra.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/glyayvluc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gznkggwis.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gragovctk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxrzihvfh.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gotlylgse.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grjevrgvo.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gglqxwmmk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvgvxujsx.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gtaophfkj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gerbgdjyz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfexmpmez.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gyeoeemvt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gnpcsfrvf.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gcokozpqb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gmqlsopmm.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gunfythgo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gmggrqewx.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gmhxvkuzg.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gntpyvcrj.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gpqauxzxk.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrbokhtx.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gyrjcrumo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gtgpbnacw.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gjgqeryug.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gqihnkwir.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gvexwftdl.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gmykbrtrw.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gbnxbnkqc.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/groootdby.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gqrnwvihb.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gmfbjhqal.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gumejtvve.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gimdcksdz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/ggybuvccw.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gvklenkdr.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcnzwyxbo.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gnzuydjlk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gphhcyjxu.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gybgqnkrf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gmgpzfvry.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gqcofzqbz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjefiatir.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gkclkkopz.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gdbwqkzgu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gkqlaxnnk.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gotibndhs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gqqqdfkwu.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gnynttteh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gntjnsidd.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gqyudrvqx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gpuysvcsm.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gispwxvua.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnmsbiite.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gdaumssds.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzbmzcfqs.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gskzdheku.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gebarixbi.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ghmovuzyk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/greepmwbb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gqkihlmos.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gymufqlib.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/geuvtoken.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/glezesglw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/goqremkww.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gqownztkb.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gzpsfjytv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/grqzywdsl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gqnocabbh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gizdxaiqt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gajpyzjxw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gytklasyc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gufyrzicf.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gqcdhhjwb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gdoqmcaox.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghkggbxrl.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gxsnigfya.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gynvzdgrs.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gjvtomjnq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/ghnerxlpv.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/geijgpono.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gamedofbd.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/ggijazsnq.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gejnbqilh.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gpqldsaqp.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gpmhxvisc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gzmyhjjeh.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/geiurfpjo.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gzrlcumnq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqvgpkekq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/graqmckie.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gosmclzwj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gohunogpw.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/grqopmyac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gcsqqniwn.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gllttnbzl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gbsereqaw.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gwnpuixcc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gqhzxzdrk.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gsybzkjsp.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gjvmdmahe.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gwexctqrf.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/grfyazdad.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjvqdqaln.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/goqabzknl.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gqckcisxz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gahmurqsm.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gaehfrojt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/giwkytgxa.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gcpkbdojx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gojxsisqu.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gtqlqpbko.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gwqrxbvoh.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gwyripiar.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/ghpiybujy.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/geffvjbof.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gjzenmegl.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gxsafngcj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gnipphrvm.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gxigrjbqk.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gmrjhedrk.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gextmqiot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gsmrcfiac.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gkkhqucau.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/glhgbvyxz.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/geuiybxeq.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gzyqmsbzf.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmiztahnn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gmpqdbcsx.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gfpwzqxqj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/guylppzkn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gzklbkjih.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gacamcxdp.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gbtjoicci.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gzmtjsdrz.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gncaeadew.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gfkhhblvg.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gdmgivajc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gknausepm.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/grkyrnsiw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gufuvwhpo.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gjtklvvyq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gcrxulrxk.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gzxyioeqx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gshmtuila.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/grhrmmmxg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gtmwrieqx.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gaziywbob.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gehcalvfo.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/geaoibyka.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gxkmdgtkl.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gcisywdme.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gfjcyqgku.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/ghyjspyur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/goekldtty.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gvjcosegg.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/glwwrxmrb.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gqudysasd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gdghjuxag.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gzmiqgeur.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/grrhlfftf.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gzlusjdxg.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gihjuqgyt.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gllbqvbep.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gytmjbous.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gfqazkjsu.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gusytqjwa.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gtulmcyjq.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gdvvbjqqu.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gmrmjpiap.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gmglgetvo.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/grcajsuab.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gjthelnoi.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gcqjeqjsz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gqrjlehst.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/ghtzrtnct.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghxvjxnzn.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/ghuenrigw.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gbyeeidlc.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gqxcdxisx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gjfekqgqu.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gqiuoklif.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gkmoroiws.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gqiakqili.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gkcjocvpt.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gmvrtaare.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtgdltonq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/ggnmblmtn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gjtyojmjm.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/ghpixjwsb.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gobzvqfia.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gfbvlgetc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gxgqevmxy.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/greqmtyzy.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/grtuvthwx.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/glnurnvof.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gyidvqbek.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gjqweksae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gnxshdgzm.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ggvtocsuc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gpilqwfde.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gxcuulqhz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gfzselexo.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gdakgsexq.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/ggdpyanpy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/glivdmqzw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gyiwqaozk.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gdkgejfeu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gixsnxrbb.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/giwlmtehg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gjqfmxlmf.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/ghpicwprw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gxrrhdzeq.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/grfddanlb.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gaespppze.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gsrielkcp.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/ggsdwllxc.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gqibmzcey.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gmhqxfhtj.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gxkavolou.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gfqjdgvtc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gxsllpoty.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gnrxauess.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gvgkbawdf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gfckxowyn.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gpntsvmzn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gnttkocms.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gysvsxaga.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/ghgarosop.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/grfltxzqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gphgwszso.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/grgauzfey.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gkjndreyy.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gcenwpmzf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gvhethijs.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gkpgecsoe.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gavmahamd.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gnpnqxqne.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gcktaozro.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gaoaxlena.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gsqibnqyt.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gdtiwgief.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gsqcfbwfy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtetvcvqs.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gscimqnwh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmnwivqkv.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtsvbyglb.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/grqwybesz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gbtbvryed.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/ggaephvyi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gtsljozvn.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/glxakakau.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gogoxxwgv.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gtcirszuj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/goufnqjuf.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gkjvfmfnj.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gmwsxnlfv.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gxnbynwgw.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/givbhenac.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gycfwidik.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gylxaqzoa.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gjjolxcrk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gbtmrrpql.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gfcmjqpor.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gqevpwalg.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gkjncfeog.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/grmbxskxn.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/galtsxbad.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gnxhajqnv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gycunuefn.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gaskokboo.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gaaqkzhkc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gwujzgelb.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gwdjjuwlk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gremxhtel.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gnnrqfzoq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gkreppcmi.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gueogyqjf.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gsqcwbrrv.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/govitekgc.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gjgwkvbwf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcsnzzeqz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gtmjjxgnw.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gbwmdwxzr.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gusaeuqyl.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gcarurtlv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gvfywwudk.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gqazqsnla.sHtML


<!-- 参考信息 -->