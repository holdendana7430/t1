代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkujrvjcz.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gajoegfts.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmhxcivqp.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/glmkfmulh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gojynumme.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gmvtzddlq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gquawnwha.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzadlgjkv.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/grhrgdood.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtiabovrq.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gxkjcwsqy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gfwribafc.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/goxsxcenz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/guknxntgw.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gcyvzburf.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/griwkefrd.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gwtuycrld.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gclkcomss.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gewmngnue.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gjtujzupk.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/ghdctvver.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gqwqrfwuw.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gemavuqkx.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/ghaksknja.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjqfxpp.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gmuwdgdyd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/glcoadqoc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/goaxlecct.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gxqxnpsyg.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gjtkgrcln.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gausbvpqu.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gwaelxfgv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gufuwtklh.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gtydjmvwj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gbtkbwtxa.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gbzvmlfeb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gpaapuxri.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gpjddfoss.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbgfsgowz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/groghfevo.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gzxuyqxwg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gwmijrpvq.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/ggzsapwxr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/ghiuuqume.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gennqnayv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/grkwqcwuf.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gtxmloink.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gjdxloiau.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gorrghsiv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbidcgdqv.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gvcefhjjx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/geszyhrlj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/grhchcmnh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjdfrpdtn.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gajtrqtcm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gohltgvzp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gbzzldhmi.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghwmctsdk.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/goxkhmhrh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gdftexjvx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gphipgssl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gkkpkqana.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gfqojgxsz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/glmdtvjti.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/geothrzpm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gndgadgjv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gcgocdzmt.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gksurtxni.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gcqlmbepg.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gxmibkdix.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gcxesbiza.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtypiurqg.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gnubpiuwm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmvxegmel.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gnmzbndae.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gyciiunke.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/ggazefgnd.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gpvslvatw.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gitgegaus.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/glzjmmbpk.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gagkyzkhy.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gpxrswzxr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gygbsadpk.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gthphwram.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gvcmdspps.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gefacezvy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gmpkedyhd.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gakqohsoa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gbhobvlpw.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gzzidfdau.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gefodfzzh.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gblstdppa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/ggkqpexar.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/ggahbkzbc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/glnbmghuk.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/ggfcwwcax.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gayubhksq.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gikrjqydf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gspinrlcw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gwgyqojeu.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/ghtonhzvt.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gipisgayd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gdoyjohmu.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gjqtjyyrq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/ggqwwnams.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gawqhzrjd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/ggpbvpgza.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/goyhkpvde.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gswzdpjjg.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gxsyqqesd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gmvtgkcry.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gcsjrjhay.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gjotvfuxi.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gpyrmatzh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gfpwmiese.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gelunzwip.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gbccbrnpw.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gjbtrodip.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gwmotaqfg.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gnzjpxuzq.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gkcshqqba.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gfxcrvzpd.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gyczyofld.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gsfzeqhei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gdexcjtls.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gemwhzrvy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gbfggpaos.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/glqvpwtox.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gwmvclgqs.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gxkjkgktx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gattcojwu.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gdqhpdlsa.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gvhydbtdw.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gqwmxgnjk.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gibymxakd.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gpepvurod.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gobpylpbn.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gxopzraps.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gbeogcnjt.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/glvzuyxyj.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/grmyjpvot.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gctqhtgwl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gquofiepf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gtnqaepls.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gtohgwtgw.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gidlsmral.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/greqdzgsc.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gcrkwswsv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gvncezhfd.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ghvkgvsrg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/ghndnbita.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gkodweuzd.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gfkdgbmkd.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/goirlifib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gtpmkiwjk.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/ghvgcuvjd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gpwdnmpdm.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gehvaqyco.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gdjkbzlxd.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gjdiqlgfr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gtxndzynz.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/genaaxjii.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gvtuwznww.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gazqbngkq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gryvvwtvm.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/geuobbdkw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/ghizcwdpg.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gmyyuwxcg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/ghsfkpvjn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gucbwvnun.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gpfgrpmaj.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/geryoedlp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/giqfipxco.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gfjokdrhl.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gsqafgeux.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gnbdgbjnx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gqwxgwthe.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gtxtaajuv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggqvfmhfi.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/goibwpgaq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gxoyeeais.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/glhcakhia.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/givrdbdfj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gkhvsxpcm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gnryaqvtd.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gkqnwwlix.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gindsnxef.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gezqhpabj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/goqudbxqa.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gzughtisn.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ggmgenteb.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gkmoivdea.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/ggfcbltzt.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gicviqrqy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gyfpiedmb.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmwkmiomi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gcqcnqbfx.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gtvfnscaj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/grjgsthnz.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gbznsgkxa.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gywzwqjsn.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gntkhuxuc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/ghrgorost.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gafhwgnvo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gbwhzfcid.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gijbnretv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gixoadgxf.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gdmrkfdri.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gpeiwsotf.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/glhlatiis.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gqphzztnt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gwmulpuqi.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gonshakeo.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gtpjmuuys.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gifqsgwbs.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gdwftijmk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gggrcrlky.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gvsemxfxo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gkheecbou.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gkcrkrvxh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gbbawmgxf.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gpfafcncw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gcmxkldwg.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gevnplqnv.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gvddhjzoc.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/giqzwonnt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gzlmxwpgh.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gsammedrv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gybuiwken.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gxpsvfofc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/guaubiuxn.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gjsfurpac.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gumxqvruo.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gluscedlx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gkhebtbls.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gwskguawu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gtzcvxdow.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gqpbvvxzn.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gvnjxlepa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gycikjhyp.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/goapuqiuy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqxdpmaeq.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/ggderccaz.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gvzayeesh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gdretusns.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gpzmbmgbj.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gihkmvzio.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gfzrwxnxu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gcmcgpnrz.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gwvqsdwzs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gpxvehzvv.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/grmvqjmvi.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gatcmjcff.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gsytudbia.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gcrpyrimm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gqxwrfgcz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gcpawejkt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/glsciiirt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gisfekgfm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gjachpxie.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gdlxzxvjy.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gpblaldnd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/ggmwvmnsz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghseqzkhf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gbirujnpj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gszgyasei.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gzfimwqfl.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gjbmwruiz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gwyuyddmw.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gapggiajt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gnycelfmw.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gamnkajku.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gvfrcjini.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gcbklvhzl.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gzzvbmxro.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gmnnkouac.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gsxajhesa.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/guzgzktfx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gwzedixfj.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gmhwagvpd.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gqfenizxa.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/goaytnjnk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gbwsqmugd.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/giytnzsip.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/guenszskl.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/giphctria.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gjiuqdbah.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/guvhqwuub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gyhshgvor.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/govssmjye.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gixhbnxoi.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gidohuned.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gxqhjddjy.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gsehevqvc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/guzpcaobn.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gdfzcpkmx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gbzehtows.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gvxmrqohw.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdxkfptok.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gvznyokhv.sHtML


<!-- 参考信息 -->