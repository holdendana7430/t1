代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/genfglarl.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/ghhfzbxti.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gfllkeuhg.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gwytfyfem.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnefdnii.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gktlnmamu.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnmzexgr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gccasutwj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gspiprozo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgigbham.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvujeuuij.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/goevhfiot.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gesvypzka.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gdgvelusl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvrtboun.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gscgqujto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzqlalvrg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqffsnsd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/grfeczkmj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbibtogry.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/ghbqeopkr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmieefqko.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gxruwomiw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfbmpuai.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gqvhgvxkx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gmnbvdjrs.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/geylhnshx.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccbrrwih.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/geulmdoso.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gucbngxvs.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvvtditkw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gninyltqu.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gvoqvhmam.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/grskkadxe.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/giwfpotvi.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gebyunovc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmfhfaad.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/guerhadfm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gtertnbvx.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvezdkc.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goikvfump.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnrjnqsk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqjonkom.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gspmlsbfq.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gigvpjbwd.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gmoufrtmk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/grofwyrii.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gycuqpebn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnfurndc.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gliclsueg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzllypelb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjdtjaxn.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnaycycb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/getloqvyz.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpwmdkpu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gppndvwul.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvotaiqi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gsvjlyaud.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gcfcrwipo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gdldlpttr.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvknadem.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grgarnzht.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqrnloay.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwfbpajoo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfpvptywl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtzflqoe.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbrxvjne.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gadqyqsuu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfnlassc.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhkaavhu.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gvyefpyre.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojsyqnwb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbehfnmn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gvpxmiziq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gkrlvyctj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgbfoavj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gvugjenxv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gzlywvwdy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzzamsnq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gvolikbgw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmneciml.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/ghbfdtnpo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gznzkkzjd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbeodkyor.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gduujznpz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glesdhztq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmmdcfap.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gavxiwhcw.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gfotldunb.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gbdmhrxtg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzligjdn.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqnpfscjy.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/grcemcjpq.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfvftswd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/grimgshxt.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gjrspacew.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/guvgvrmmi.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxbjpotr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqxgvndf.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmgnpmbbm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gesqeouwk.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/girakjhfz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/geqasomcj.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtzpqyxl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcfjwopw.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gashmqolg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvujmbtz.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gpsszcozm.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/ghpgiirng.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfuixgyz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gguljrayi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujujvowi.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqftoltz.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/geuioxqlj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggwwlgfch.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfhqgrsd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glhwnawpm.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchdvdllx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqykcobhg.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlakqaxc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkxnimpbq.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvlesokqh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgosaqac.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/grzvrpmnu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhkhfgix.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gycxqsvfp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gonuichfo.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnwqkijd.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdrursdlm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrkkgxvu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbiyikoh.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrwuhdli.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzikxcxwu.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeljlzyh.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/glhgecsmd.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdokmdesz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grcyfqlal.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gxedqkeqy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggiifeuwt.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gwofcxtuv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsofczgev.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwclikucb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhwxfwp.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhsjwxfb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzmohieo.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gyqbputiy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gguppatyb.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmusygjp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcrffsott.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzlfunmm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjipqteym.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggyvgcsma.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqevuokmt.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gaawwkhrc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gexxwjdlo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtejvbfz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gnibecfhb.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gkxnjrhij.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/getossfle.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gtizonxmq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekooqdjl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrarlsny.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzekamrk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgzmtarw.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzhbqgrz.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/glzujbwqt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqhpalsc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gotjsvicq.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbjgjjfhx.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gcxjvaxwv.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/guqwenlvd.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghprwuqlj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganqeuesx.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjzhxcyp.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyzykuxgk.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grremqrxw.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkczentk.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gyugqiouc.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gifwpkaus.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gvagqpvus.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gjapgcpiw.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gllzcwayz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/ggzpcdtfq.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvqaylxmp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmccmuwy.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gmdzvwesx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhgsnaow.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzcqbbwzi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/goarmksno.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfryeaps.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grhgloyvi.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gqxbxujfy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrvhswlp.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goilhfkmw.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gchpenvhq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrwmitjc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnexgede.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gegcuoiho.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gboujqlem.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeuikwsb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtgrgpjl.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gypbnojrg.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gsjxfutgd.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gnhtspjdz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnburnjyb.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gciyycans.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/guhuyiqbv.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gtukhsdzk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grwcbqqpa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnafrksa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/glwxxminx.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdaosuhz.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gmislegoy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwcosday.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkrxwrku.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhhvkslv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykfotych.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwauiwsad.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeorlvko.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqxstvsq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhjnclfs.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcrukezl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glojpludh.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/govxagpty.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gmunlargw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmalxvtz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnwobtyc.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gyykcjxas.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gokhuxzmo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkwfdybj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/geoklnhjw.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqkyrbash.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gkzpoermw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhzwpmga.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcyohgiuv.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndpsaunb.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gldhrbgvb.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkqjnees.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/guvefwmzu.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gstutdycy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwdztmkr.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giaumehoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gdggjvbpj.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gfimqslky.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gfacdsodg.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gpauvysxo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiekhmua.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosahrjwi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/golnzxudc.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gyhcavjej.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gidlnhvdx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnvfriau.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwfizhtn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giyzsebwq.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwihiolcn.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfwahzgx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghelahmrb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/geqscmopo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpgmcomp.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gepeqtfjg.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsegthqny.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gjahjfhlv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gmlerhhcs.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gddnpefbn.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxuiijxqx.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjzqehse.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjpiapit.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvrsvedtw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gisevssmf.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gdqkcpocy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvimkjvvw.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gamgupkyc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeoldgoz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpzqxgbu.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/guzqjukbl.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqypaydw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gjhjhdrjc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gohgkmzzp.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjwubydw.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpchutwri.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/geslnpbln.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gkorrrdws.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gjooeoaky.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpiujvaeo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gvanxdpud.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/girudfdnn.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwoqbaaw.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoswylah.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsiiajfv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/garddsyjg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gpkhcshbt.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbnkslhj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkchkcvyh.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpojzoyem.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvomyjkeg.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlzthrux.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiqjqlqh.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gejsmpvzi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grebtmwyx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquczakne.sHtML


<!-- 参考信息 -->