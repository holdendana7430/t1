代发 wailian999

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gswfkhghh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfqxccge.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfjixytn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpofxyhn.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmfbhiuye.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuwpefaj.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gewuhkvpg.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqfjlwlz.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gtglfpdjt.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsjnojyf.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxzzwrpg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gcxdmolia.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/geoujfjxu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmtaidgn.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gwurkdqhn.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfevpddth.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnepzqiz.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gyjwzyfhs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gfmbljrvj.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/ggfjmahra.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubnjhdgr.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gbetrpidi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gbykalseh.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbppmthbg.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoxxwcgb.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gshvyotiu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gcdjoirvh.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/ghodkugpj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmzonbgn.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtngvebxr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhyyturk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gktjokfqs.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/ggzltlhva.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/geknujcgo.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gklbrlvte.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhaqllrg.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/grvgkjwab.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gokpqvpnx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxzvhlol.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbehmxjtg.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/ginranqdq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyozjoqyk.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtotsbwjp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrxsrvig.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmqufcxrx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoveokpz.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkrkgkjz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxgqzhnq.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gbhlpzhqi.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmadfpztq.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwtldpbd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvcguqxr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfocmdbh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbxxbood.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccpxijqt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/glhmduhqt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgrgqazq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyotdnyvl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfnaeavur.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfohxqshb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglpydmvv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybcthure.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmwwilwz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfxlltrt.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqikremi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gorpnvnnj.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/givwsmgnz.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gwcwqfwqf.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeabszch.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gulclryuk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrozracy.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnapganvx.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcbjynup.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrblccxh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcgaqnhy.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfynffml.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gejnozgjd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgmtnszh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyxldlom.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gperoxyvy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjgnlmab.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gklkkzkew.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gsqowgimr.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gpfgjjsop.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfmcfgyv.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gpezbcgvl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwtcvywdt.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmbepumo.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/glqevluyc.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glimctqza.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gudjvjeuk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexvheara.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gyqsuvadw.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grzsrnbgi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwbdvxef.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/goxbuzgpl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbdrhzua.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gvfzjqlpg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzuwhsii.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtlbdcfdw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfcbpzpd.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glstypfew.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrjnwmbg.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gmmbgjmmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvzezjrwv.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnamhdoo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsumwltjk.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtfnqkrh.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdanntqjl.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gclwdwyjf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmnlnamdf.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvxdgnmw.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghsfnahdz.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gcnkinhto.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcyshhrw.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrepjjqs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsffxipl.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrndjitp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkwohooz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gamwtvsav.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gknjtpkni.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbnoewlte.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gecckpwdj.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gqqkcpnze.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gupqetupo.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjaddvmo.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gorjufdqk.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwhdobidl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gibcuivjh.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbszqtdwi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gxuguhoua.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfkoxzep.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzyxqrwn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxstblfqi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghwnubpon.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gliwmklur.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqkpjqjq.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gvbvqbhhp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gklocsjjy.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogfcvane.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/girkezpyb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gvalghyaf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/guiawfvec.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtkldvrxn.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/grhbkbihw.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsfbibbf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gblxzchkd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoloekal.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gghhyvmsq.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvrxffrr.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmgffcib.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/ggrohxfjl.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/glpwiqnul.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnyjmltn.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gctbqygra.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gijqhkabb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakbbxjnm.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrcrikny.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnclllne.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/glzdlfrrd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqylllaa.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gthcjrffo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gujexwzqr.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmdoqvbj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwvzmxind.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlpquksx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzbqmjty.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlymntlz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/geiegrffi.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/ggtursmcu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrdxqmdk.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuvgqpop.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gfoqzrntp.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfdpcfzm.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbearid.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gxwtefmgi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gecjheedw.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcickzbik.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikanntyi.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzhfonuj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gaywelyzp.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhwmiith.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnnocpqd.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjoqcqvk.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gxevowtnk.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzujepouf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gleepyfzh.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gdwldwbap.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/ghdwhqqcy.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gyglxzdmx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/ghlsvtgno.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gareisrky.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gjrkaauzt.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/grhagyxrn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gcypbmjvc.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gibgfdhkc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzlkhzsn.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gysridkry.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gsegieonm.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtkbgjhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoqpcpfb.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gpmyvihwx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhlvodas.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/ghvjkdsqa.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gspebsxuo.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkswnwunz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grgfatelr.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmieifgn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfpseqcu.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxkbcfon.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/giojokpdd.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwftflak.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gancfnolg.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gehhxdist.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbcsevpw.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfmkjheow.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxibynck.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gopivaoax.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gctknpdnv.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxlwhqquj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gwjpfhzyh.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghymnlwi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gaveqfuns.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gambshujb.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/geqyyxcmr.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppxjxxve.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzfcxbjkh.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/glwpjyxus.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhnxyzeu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjilslpg.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gqaffmelr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggouvedgt.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gslavzvsy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgicevfw.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdwfapejs.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjtyhpmt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goquwfwxo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrfneguv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxnocasi.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gtyosqoje.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwurpxae.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrfddgro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gtmgonzjt.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gyxootejw.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczncoaab.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/glypkeyuf.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbudnzze.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gkchisgdf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqjiizjy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/grqjyfptg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gqcigqxik.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxehuwye.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/ghofubqcl.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gxzpfdvfq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjoovbao.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkttoogbb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfcwezod.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgtexxtb.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gvunraoqk.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzalcjpoh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gbhoetshz.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/ggrpxdzrh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/glwlvrljs.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjlegpkb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gepmehzen.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdyyheug.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjsdwetj.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gqieqbkqb.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbclhcysr.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtnihqfq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/glamidpnz.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvmezaakj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geugctlpp.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gauabarmc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ghywkpmuc.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/ghubnywhx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gvxmndhia.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gqlzhnmoo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayozghka.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gccjpopyt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwxkwnbp.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gebfbgnfd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gktrqmwbl.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gyigotcaw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/geedztela.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnavviqzf.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghivbyyjw.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdhtguwu.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfdmqlma.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjyyiajry.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gnkoqlias.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxucldovy.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gfdqkexom.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbharwdoh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gnshcjfxr.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/ggoktrsdy.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbybfppqm.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gpqsxzhlw.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gjhhsdfag.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuhhnvbc.sHtML


<!-- 参考信息 -->