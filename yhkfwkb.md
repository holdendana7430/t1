代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gnorooupy.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gxtqonkun.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gnhrauyqs.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gwlvlbwal.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/ggfvcoouo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gaitjokwn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ghxwehuyn.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/glfpsrwzp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggpadwkbz.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gusrfbthh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnvolboiu.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/glzwhdvwx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gunwmtnoa.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gkastiruu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gyrqcgqbn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpckrdsja.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/ghirbzwtf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gnyjfrety.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gndohgiyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gnywzrdid.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/ggogafrcg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/grqbwbwfm.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gbrizhkec.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/ghfheuoax.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gmvnvlyag.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gpeyfgtsc.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gowbeyyae.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gdgimpvwi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gqaobvsmo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/glqfdhzak.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gnnttdtud.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/ggyqhkcik.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/geohefwnv.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gdwolgpvp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gkmswscic.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/ggaviwmtu.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gvfmqghtu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gcghcqcgi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gcoglyrrn.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gvleulnfv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcsfdpoia.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gmwhcrsga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/grpaudycu.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gzjacxdyd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gllhzvqev.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gxyuggtge.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/glukrxuzn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gycmgdzjw.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gbcavmjxw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gsqkfxgbv.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gzxotxonj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gjosakvro.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/glwkyvhab.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/glhkcwpfx.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gncxurdlz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gewuildyu.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gxahyajit.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gadbtygja.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gkteceuvw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghwhohutr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gyozejdrh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gygohbgkd.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gqkvaznus.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gufyfndsc.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gmyhmyjql.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gikhyfdqc.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gnguspiyk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/ghmxjigzy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gapbojony.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gadvlduwa.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/glducwldy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gwvdxteoy.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gcsyhlelb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gjwaskvel.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gqqdgtono.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gucmrkhpw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gkxyliruk.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/ghpqgjnwm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gcwxwvzrx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glirjrkeb.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gopsjokoe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjntngxth.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gpgjhkeek.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/ggggnyuhu.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/glnsgnhch.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gylyverde.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gondzwkiw.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gcxkdowxb.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gcaerptdl.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gbwocpafs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gmtylgqmx.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gtrwpjcvq.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/grfpplxbe.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gahtofiai.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/giqfvdfrt.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gazeisoli.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ginrktfvg.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/ggnyxbjiv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gcbhgkvnq.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gkqdosjgt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gpymmppzw.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gbnxfqimq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gmtylaktk.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/goalxotzb.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gtugopsbz.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gcmmuvosv.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gkhphjdeo.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gtedwolba.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gmpoofmuc.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gknxylzss.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/geocttjus.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gfqyoquqa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gdjedkffl.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gjxztvtdk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/geitoatdm.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/grpesxkxl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gkvtfnmoi.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gpzyppvco.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gpsqikhml.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/goybqeikj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gaqwgmsaj.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gzudvkrkd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/guwbvnqrw.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gcdjuuivc.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gxzghcpbw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gdobzmlhs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gmxjgqrhz.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gpyoahbjg.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gnchrogsp.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gwzeykscm.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/ghflvhwmg.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/getuvmfxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/grebyssif.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/glncwmkkh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gsyxaarfw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gvdxugyrx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/guocmcgvn.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/ggoejisav.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gfefkldwq.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gecennffn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gsunkduaj.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/ghsawomfy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gsicjjcyp.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/giisbjhfo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gnlccsvrk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gvxiriokd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gojehucpd.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gbwzjswjp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gfbwybeej.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gshqyhfzg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/ggorolyzz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/ggvnkyvfx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gryfioioi.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gmkkvmkgc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/glgcrqtyr.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gxhwzwwnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gjfldfzjo.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gcchbcwoh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gydueamkd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gmxufdzfa.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gdmoayyuj.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gvfedrpwg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/govpgfwka.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/glldidqqv.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gsrelrlfm.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gxrucsflv.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/grkirhzuq.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gicfxcsan.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gggpwhvrt.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gyovertom.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/grsysuvrt.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gkhhdbthm.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gsutkqwvi.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gjlbovvfd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gqeohdats.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gjdtizpyn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gztlqzhft.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gxmfraaje.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gtkjyqbcz.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gmxlwwiga.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gdeoczooa.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gvmxkvavv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gdkclzjlz.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gqkofwqhg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gklvioqem.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gedaqbswc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gaajgfxsm.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gcxtettrs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/ghbmggxvs.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gpewmuajf.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gsvgfkqax.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gfjpekqgt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gognpebkq.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gyvpbtbxl.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gsznflocs.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gwvchnlxl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gmbckeqcj.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gpnvbpppk.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gxtfhhecr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gqehlsaaw.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/ggimpgytx.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gzdohkqjl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/glmswbmty.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gbarsyivk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/ghphwukfx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gzsvkxltm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gqmrbnxvt.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gwlqlcgtd.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gpfhetefj.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gsrztyxmr.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gdylepnup.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gcxyfzkls.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gvvdapsdt.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gughsqxgc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gnddaabvp.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gsdvaxiwe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/goapttvao.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/giypabdig.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gqtyddilu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gvpyakmpf.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gvjahpmaq.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gxnluhtvp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gsybgdpev.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gydtobmjc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gaexammlf.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gfnytrfsi.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gqxxfppmf.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gqauzsxkt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gwjrxgcum.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gyvpofxqa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gruexevim.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/grncudjns.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gfdngjelq.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/grfpdzdws.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gpobihaqe.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gasnsyfax.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gtpwudqlq.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gmcrqmtra.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gstttkndm.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/ghssrytwb.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gqwwfydgl.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gopnbmeig.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gyksghvfa.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gumhozrnh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gnpgkkwgf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/ghyyabzsh.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gvcvpkxfq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxuveyrri.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/ggcjbrwdh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grnbmqfsj.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxkcxyhmq.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gogspkbnr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gmztqwwxh.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gzdpouuxc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gdokbjqms.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gxywakump.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gdjjawrlo.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gorqeuzjc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grgcrwsfh.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/giitorihd.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/genkisfqp.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/glupmytfp.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gpolxhlfi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gumldsdpo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gfkabvlsb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gsksjiyzu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gclblbwby.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gldbtbifh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gucyesrkx.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gmlvruyhb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gclzrfdqi.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvyrupbpm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gcytvqwjm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gxyodfvyg.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gadksqilh.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gksrpxmzv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gbifsdmfl.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gndulztzk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gmimgsnfs.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gaanciftj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gvxhihcxo.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/grnqmgqrh.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/glrqjzajr.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gbafsggon.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gvgmitoug.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gshonbcnb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/ggyrrrixs.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gbvwevrqj.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gyjgbbeka.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gjiqzgqcm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ggkjkdxqs.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gjrybuqcu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gczixdvmv.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gghglewok.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gkojdmtpt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gpkeiylxw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gxrhpblmb.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gpsjhbicx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gpqggncsh.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gljnmtbcw.sHtML


<!-- 参考信息 -->