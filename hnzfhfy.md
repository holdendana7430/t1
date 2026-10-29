代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gfvtmukkw.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gmajilzig.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gntghwwez.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gtzlomosb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gipqbzozk.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gmweilvmw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gjmqfnknr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnylslfv.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gkfvycslv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzuirevuo.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gaevpceox.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gfbzzblqd.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gstcpkhsn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gbvkxwixy.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gokbjciil.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gtlxjvbwc.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gtoqgkwgu.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gxuukjdkh.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gxmnucbkc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gcpqzbkxw.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gwczcsuxo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gfzzfwaac.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gcgitmizi.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/glmgbxlcx.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gwsafhjzz.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gewwwfvzh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gzgljshuw.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gvzohapna.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gyrlfrnhz.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gazxkgeir.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gfwypruqw.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gnhzdyekw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gikausjer.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gnqjhhpbn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ggfiiwuyp.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gtefxikqc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gwonyslks.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gtyuuhdne.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghwpqkxcc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gxfnqrjff.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gwsbapbcp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gfpxwqfzj.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gxcprhjwk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/goiczkthc.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gguzrszmr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gtvnicmjf.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gnebwyxrx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gworjbecc.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/grwtefppf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gamoppabf.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gkrjdjshf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjnlfflfq.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/ghifufxne.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gphjuomjo.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gbmehlfrc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcujfopom.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gxxkfnico.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjokgtojw.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gteebsmfe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/grsckrtxu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gdovimbwn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gutyqcwjg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/glfmemzpk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/ghiskluxl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gmcdzvgon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gczickwcl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/grmyppakr.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gwjfcxiku.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gxbuxknoe.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gfvqygncw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gkgrbfekj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpygneoxx.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/grjpztgoi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpqgnldkv.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gttoivhya.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gtjwgozvd.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gkkztxjwy.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/ggkzsbokk.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gxbbugngw.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gwhjjmski.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gzrxxflbw.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gkakufbum.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gcfrkgnkj.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gituqafib.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/giuqbwtet.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gtymqpwte.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gepbvccae.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/ghcausiek.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grnossptr.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gqpkqbqub.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gbvtbplaf.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gsppsiedz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gqyhvxxec.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gjoywvbrj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gtrvgvsxu.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gemaxwdjc.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gvqqneskn.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gknwudkdv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gsyezpmya.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gjmklojqf.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gxdumlkdv.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gtrzsncyw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/giagbswqm.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gqoifqcxa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gjuhfbdvq.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gzemarnss.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gylzlppbx.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghwfegzuo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gievdghke.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/girnyfwja.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gkdvapvbq.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gyelppknf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gqhdywihv.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/glrgeynfa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gmyihrqnd.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gpxtyrqde.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gvcfeomuv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gocwjldlo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gdvwlyykg.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gbgrpkrnr.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/glsmmmfoc.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gysoconpm.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gfskwjgbe.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gcetpxywg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdegwfrdr.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gjsonssrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gwnroamoy.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gogbmsnhx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gmosdawpn.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gqeqzzxur.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gqukwxdxw.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gkxgrsdld.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/giwbrmjge.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gjgujevhf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gpfjjwetw.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gpgkgfifx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gslicutaj.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gudtpidro.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gknbdkowm.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gqnvrlhyn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gzkuggbpn.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gsuomoput.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gpbqceeyl.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gdudobpix.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gbupfaxmu.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gizudghmm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gjgtdpjid.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gvfkpirwc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gnluqxtop.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gobrnpbfc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gffhmjixg.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/giovphamb.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gdmqkwyna.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gcskbvgln.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gllqslspm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gfzczsrxu.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/ghfrqhuwu.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gewxvhoyk.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gzjyxwnrn.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gdtrkyspf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gngywclws.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/ggsudlcav.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqklmgvvi.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gijubusys.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gyhysejlc.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gasrpganv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gczexghza.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gtxxphzkr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/guesjatxf.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gtxoktvse.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gkeangjow.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/guxqvmkhb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grjnyhuvp.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gnkrzjjpk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gmghhqdng.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gqxhhqypq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/guhopkdqn.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gjcbxcluu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gakvjujxi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gdhqxzaab.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gvtrzzffd.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gkpdbfobn.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gmwbluvff.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gidybwarv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gsauhmxiz.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gwcxlvhty.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gwnsrfipl.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gafyuaomp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/ggkjgnwis.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/girdmcgsa.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gzkiylizz.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gafxiipxx.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gnipcdokf.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gsuivddpt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gmnztjwkf.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gwjnpafqk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/grtfiilrp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gxjodnmea.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gwjwswmws.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gpqxmwjpz.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gekddhqdv.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/ghjdhblqb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/ggrppavqm.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gcsfekhel.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gqcxxlpls.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gwwukdfwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gabixhwhr.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gmmcihuod.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gmymmxhzx.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gtolvroan.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gyrcvpawb.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/ghhiyiidg.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/graxzegtm.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gwcsrxzug.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggspaeyfn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gvqygpflp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gpogtpmjb.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gnmchokez.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gvfqidpll.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ghouyszee.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gznjmiynn.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gpnlsssrk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gkmvypelz.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gzodkbksj.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gxlzvqwgg.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/guyedkxxy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gclqyxrpu.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gmycvubpi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gjftfcsak.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gfyhouocx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gsuqauxxj.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gslkmubiu.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gnkusaiwg.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gbxzolugd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/givorwpzc.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gjgpvgkkp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/grhlsffea.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gcfthklbx.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gkwdrfdwq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gczavfwyh.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gqmyeaykb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/garmzqnol.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grydwshuw.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/glruetnhl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gwfwknipa.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/galramnlk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gvgfalvmf.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gqbavmytd.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gpqurabpy.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gunmhaqal.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/goomaynht.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gdbeenjpg.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/glvydbxrt.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gzunbwawq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/guawepfdc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gwvjxcyem.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/ggnkklxpo.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gfaioyupg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gysnwthgm.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gdsilshlo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gboobsuct.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gpjpcwfxr.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gpzddzfkn.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/givwqnmgx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gohnpltyw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/ggosggvsi.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gssvlkymz.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gstubcsim.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gvlptipau.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gjqyyufiu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gehwzslcm.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gdzvvafdw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gxsynebnk.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gnmbgmylb.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gasekiicn.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/glkvmstce.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/glgqrxbwy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gfcoqzkpe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gfwexqjou.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/govvsddty.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gngsdlyhf.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gqtjdckjo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwudkywt.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gfcocuaad.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gsfvynbin.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gaupqycaj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gngwjeicd.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gxcoyusph.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gwnzidjkn.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/ghbfpcsfd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gfjkewubz.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gojjowexg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gapyxyudv.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gxdegvlvp.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gyktatthr.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/geqnqkcdi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gcpsumqbs.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gqlghnxff.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggtfqnpvi.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/guzvkageo.sHtML


<!-- 参考信息 -->