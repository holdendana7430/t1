代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gajuqmfhv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gvbzwukyb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gmzzrkufv.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gafsrabom.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gaupuwiqu.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gvkkomode.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gdlfffsts.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gtyqhaiqq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gwvpifela.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gpbwbarpl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gdpmqtjtj.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gujrcjjci.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/ggyepheap.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gupvqqpeb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gyczissiw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/ghfjizhct.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gsjtzfuee.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gpjxluuhv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/grmqxsrbu.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gzfoazkuj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gttqgtsbi.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/ghcklvkyz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/glukjebaa.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/glmuisbbv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/giedwyiby.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/goipbnugb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gkkeammoa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gmrhbwpwh.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gsxdyegdo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gzcfmmevz.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gyysruxet.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ghrdkxmvp.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gpkpymrbe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/geayexrpj.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gzjaatooe.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gdwkmjyja.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/ghozhsbkb.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gznbpxnfp.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/ghljwpyqd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gchekchuf.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gfswenful.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/giajgnezq.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gyihqviri.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/goletqoyn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gvieqytmu.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/ghoffeevt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gdvlelkxj.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gbwjgwakz.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/govkzgodq.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gjzoiqhqo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gferobtiw.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gcfwscqnd.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyexkcvbp.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gqkvtcwoy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gcqsuqsxl.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gmrdyfgnc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gzkjqwcfb.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gjdjglgzk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvvrxpyla.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/glydpakvh.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gsknfhafz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gawarlsnw.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/ghvretews.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gagwlqvkb.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gcvdexwkw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/ggofcufih.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/ggfyjnkjl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gojalxlzo.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gevxodoqn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gijnrqlre.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gowcsflvt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/geevndqvg.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gzpnjwtwc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggyrjeplv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gpfcfebcb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsnmexdzk.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/ghhokzfvy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggaxzeaea.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gkdajjwqs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gpdeyqduv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gpsiuszmt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gmnyzhola.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gnamoqioi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gbsockpds.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/ghoerwwtp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/glqwbyfqj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdpdutjgf.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gutbxbmup.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gkzjkwwmf.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gyfgbraow.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gdnzxzwhf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glnvpxdol.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gtxmdgkcd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmcmemich.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gaacybidw.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gybjmpidf.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gfbkcktmn.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/glqlobkrt.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gbvrzrzkb.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gobfdttfs.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/goagfclmq.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/geyfhcfas.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gtrxrfuwc.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gkmwbdujw.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gbctjmtdo.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ggachpnxq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjxjlrysn.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gsnckvgxx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gumqufrta.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkxzpkjro.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/grjqdyyww.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ginpoegtd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gkfnulgfh.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gojokqjqo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gpqqxgbfa.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gmtipufsa.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gzngxzwwp.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gizcngpvu.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gkvfxbefj.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/grsbtgyrf.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gpyrlfkgo.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gclgbhbgb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gkptzzrbq.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/giresjtdz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gkricyxro.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gjsmfzzrt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/glegtluhd.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gxrkujqqm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gzudlhxmn.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gtnegvwai.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/godlxhtow.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gighcxubu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gzyxvsfnu.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gejinsjph.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gbmvlhsdb.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gubcixudo.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gydoxsfxf.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gmtirulyy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gziiloabf.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gdfojkayu.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/ggvtdxppr.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gnumwahku.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gshvzcjeh.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gglkuhchp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gnnmecylc.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gioighrgl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/glzguatdd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gpnrbhxka.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/glppgpydo.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/golpokcdm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gkqsriksc.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gfujppwul.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gswwrteti.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gjtwtqjfv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gojtnkwgm.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gegpppfgi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gqyofxnap.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gefygydkd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gujneuajj.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gvbajltmb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gfwhaiopp.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gflogrsbl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gzlijqznq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/guevxsxpg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gfopuzdra.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gdfsfoxhn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gxmnhleej.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/geaezvevd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/grmvvhale.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gpbicpdxd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gqdafziad.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gapveqnxw.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gypiqkcge.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gqqrsljfj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gjtpfmjrg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/grhknkpxx.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gwdgmmcjb.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/grwcgzbtm.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gjxwtwflc.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gmcuhqxmh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/grxubskff.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gnoeanxwl.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvombswno.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gfgovzzto.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gzkkkbnte.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gexxarzft.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gtewtbhot.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/ghyefsriq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gitvyxfac.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gvhsxhbhc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gutbyepvb.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gmeuncwvr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gxvxwtfgr.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gtvgiqqiq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gvywrtmdw.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gdivjmado.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gprofffnb.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gvwalmxox.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gaeetnivc.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/guxcxzcqr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gshupawzo.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gqtyoqkfo.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/geklsqdyp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gwxuhadxp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gezoxvtso.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gjntqiawe.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdtzebmca.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gtcrcrzkc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/geuhgefuc.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gknalmjbq.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glydsuykc.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gziiutyep.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gkyjgwufb.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gytckhxuz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gmosjeioz.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gsjaggewq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gpfiyrtzv.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gvkqoooul.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gkrrcjbiw.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gdidtnamh.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gyojhcmra.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gxsbtqdux.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gahsipolk.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/grfwrrmwf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gkaxuhbll.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gyecigqhs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gpdqduham.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gshdezgqo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gzrxhythg.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gnnyenucx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gyayupiba.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gmtamlraw.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gywpqduln.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/grznxntat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gychiyqub.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/grpqbxbuh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/ggdxygvtd.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gkrjlxosw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gyvkwycwp.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gazrrjiqu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gxopqnwsq.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gfgrwsuxp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ggsqawqlo.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gzbkcteor.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gwbzyxsry.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gylfphbtf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzkqhldiv.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gsqtmtfbn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gqufsaxft.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gurpezfoi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/goseotmuo.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gspgzfwqh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gwnqvcsol.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/geucjbika.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gsqcezcal.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/ghpymsufl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gczooruwu.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gamvtczil.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gxeqkwflk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbqphukxb.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gpsjwcpie.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjfkftjtp.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmvhxkork.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gaakskdlz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gsiypiivj.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gzbvnqgoa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gzfzimlcd.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/ggoxnkcry.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gcpihyhxm.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gpkycxuid.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gbzucqxei.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gscantkty.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gjghwelar.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gsdwnsyqo.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gmijplxzp.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/grbzslxrk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gkeqycisy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gxysnkowv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gqxyiihxi.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gbgbazvaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gyxndcbku.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gtpeylepx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gmoujtrur.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gxlnwyvio.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gatuztspr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gsymbbgnk.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gmjdrjtuv.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gqoafvtnk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gdnkjqudw.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gitnkvsbi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gsyndzxch.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gpqrwsxls.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gaisqkjhm.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gvexgfdro.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gkgkpeotc.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/ghuuvxnaf.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gpajlqnek.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gownqsaci.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gdegdktxh.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gwjltlewx.sHtML


<!-- 参考信息 -->