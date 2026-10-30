代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnkxfwlis.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/grxbfnyyo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsmmdkbm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/giddlipsc.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gubppmnwk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeumepww.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/glgvwfibg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryzismmp.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmhildul.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjhmdqor.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/ggdzvvhoi.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfcchlbn.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrbhcpic.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzasgya.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrycqfnm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gtppvfqdp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gceanaswz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmzixwbe.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gvsvbtgch.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzlrdcxqr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmixdyq.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaydlcod.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdryrmkrw.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gxhmcaikc.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwwexmkc.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyxquaci.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqsklknx.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gyboefpqe.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrkfhnvg.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/ganhdlssb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gachfqrea.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpebpnsy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gtmxvcnbo.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gclgtdceg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwdeibfv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gojkbtwka.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/guculpqvz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfgdiqnq.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gkihmqtld.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeobpzup.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcdqplgk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gbqpkoluy.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/goedgmtzd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gccqrdnig.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqlkqnig.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/geoqqyvnm.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gibekjdag.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golqywziy.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxytdnhh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gklppqjcy.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsohlcod.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowwjfmfv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gyemwtlmc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqfjzyqe.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpkdumyp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gfoyxguqb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gayilzclg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/grghzafae.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfrxfcjv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevebfhja.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gecdmnsxh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdysqfva.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxyyzqeq.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gnuektixv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gssisafjk.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnwirthf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqiduouf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbneflxbe.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/grmzhhpml.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejbzhocn.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpibpitx.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpxqdxbe.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gdjvtcdla.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gsyofczkv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkacfxyyz.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuuqsiek.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gsfojhthz.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gockpezvm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmfbrwwe.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gdspeqdmr.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzrerkch.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gaztamvtc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsedrzybr.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjqkskhp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvzzvmtv.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/guwonsnde.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeifsykg.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gptrvkuch.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfbaigom.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzneqpvy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gdddqawbr.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gvcrdpbuk.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqlmilzz.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzclbvqhn.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gpxmavgnb.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoiwewbo.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdheulqe.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwuylyle.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkqixjqqo.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gowfayemb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuomghbr.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjmhixew.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gaehaxxjy.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grilozakj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjjrnjcpp.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwymadhci.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosevorne.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/goqzpfkik.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwmzglhxo.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkhuqavw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwkojsoh.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gutasntac.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkidaufn.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gadjxzxss.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaopaloh.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnsbxucc.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvmpoulr.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gngxusufg.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grtnexnhc.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsapfkxiw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gatkmzimo.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfexvumvy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grsfhgcar.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gkmrujbop.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzcaqyolh.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbpffhcu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gobujtmwh.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/giffgdmkz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gfkfygccs.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/grlsyvgyr.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gdmabzrnr.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmncnqsda.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gexctmdsn.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfniudwga.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gnjwvfcap.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqjbrwzjr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvsntwymf.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gtyvkifqk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gguwltnce.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnukftty.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gsvgkjlqq.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/givpazaap.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/geltugrgb.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbeitrlb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gayfitdrt.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxrihitk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gzzhyilfx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geskntrxw.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjwoimfu.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/grikobivr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsfxzspu.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gjutantnn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gislbesrn.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhqqmnrg.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gxykiozmt.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gqdiogkqm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqszvgvmt.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzfxlsib.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokxfljgz.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiigqkoj.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gmxlwtrya.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/guoplocre.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuopgypd.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gqfrxzqro.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gkdeojatt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gqprakhaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gghjrowll.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrddqwkz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsixhsiej.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gwqdsjyeg.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvrancmxo.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrcwjnrg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqwnlyqv.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhvkalwe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcvhjrhu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gladhljhj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmtgpqvq.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkwvuxqj.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncoxqzdg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gtpvmxkrq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gowbzumfk.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gomzngich.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfntkzave.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gbqyzzykj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/glwncxuoi.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjkdxmabw.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gzcanwgdx.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpstlobb.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyaplfsy.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzttbkkle.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwdrjhao.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gpjswimiy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gwdonxtxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaotqzxr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gdxnmjeoj.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmprnyphq.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gjlhufnbl.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvnmwouiw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlctvxmm.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawcvgvbw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkvmaksp.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/guqckyeui.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gwrtodrxg.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/geyhcgcbg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/ggytulfmj.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gimruvoet.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gaommbhyb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqayaicor.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqxnimyx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpamlfiuh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltrgfgck.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryxesuej.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/ggbsfwwtr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctkfbsua.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gwzigkykk.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiydarpq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhefwodv.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/giersvyhd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldebntaz.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ganfstoah.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/groyadlwa.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvayfjqtq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/glczayotf.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gikjqkfgd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneqpmjhp.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gejcdgxci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gcqbbndtf.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfjnjnsv.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gfvbzkmud.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gncnjaftl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggvcimiiz.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrpoxgbg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdyecew.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gtpjggqlw.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcogcisi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqokvferz.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gihzyhwww.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtoelanpj.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpjqzfqv.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gfkjcpkcx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gatuxmmwt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgsbvyzp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gdmovnxxn.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/guryphdxs.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjrjycez.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gduxybvxo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeafgsxn.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzznxqfkb.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdzpvxtny.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlvrmaqo.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktexqjwu.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gpelfjemr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxyneeod.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gpwpzwmrd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/govxmfehm.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/geklsrtfk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/grynqsnfv.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gglfuiouu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/ggbzobjkp.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvaveyxzw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gnwfxpuqx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gtsmowhfh.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhvgewnx.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggbxjlgi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gokjzixfe.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gazvoyvkg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzcherti.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulnsbnz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdaqntkj.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkggfpwqp.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gcwicfmar.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gbockqujf.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdadpcnrh.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gglqrlggj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmaaowvi.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqdwpvwgi.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmigaroq.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/goefwbxmy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gupwgbuxp.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gyebkudeh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjykvahb.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gksvnsren.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyujkwyb.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkffppin.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwvdkrec.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoovyjwl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwkfbrkd.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gboeurkym.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grchkbzqr.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqoadxbse.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gazbiuxcz.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gdtdgtckf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gsijxyawm.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmtygwdh.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/grraaruul.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gislgylky.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgmsmiip.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjognduta.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgmwydvk.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiigtbvy.sHtML


<!-- 参考信息 -->