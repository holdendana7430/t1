代发 wailian999

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/glrqsqjwp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/ggfpxzeeb.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcmruuci.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwasgqaay.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjdqnwcj.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrzuyuff.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrfmwpps.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldlasqck.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gijhfhila.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gmovoxyfg.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gfbvcwarv.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqppmdjn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqdaihzl.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gddqormxi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqssishu.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqcplnme.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtxznmyg.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gzqyvlqyt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gzwczvtyr.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmnufodk.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjmmcusjm.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlazhnaq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtobhaqav.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqvvqfqk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gybqqaklw.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckntpwlc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/geweztpme.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeasqvbn.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsulmfgp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/glzjbxapo.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/glmzxrbne.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gyahughrf.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/griiralen.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpftftdeu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggytnwbnc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxrdrenm.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gsshjmyeg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwqbntde.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghecnjtfx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkzorjron.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gwmcjlvqi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gooemrvdk.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gdyiqvgvw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdibshpe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhjjqkzf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gozgxyvbl.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeoewqmr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/ggnkavnpo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtgpnmkb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gmxmvcfhm.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gjwysyxpd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcdjamxf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gswifzqkz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwqkpbho.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsocsvql.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflafjwcm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gnryxyzlr.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/garxageui.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gpqkgtxbl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjolueje.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzxtxbok.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gayptiebr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gvylwuhmu.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwecyroky.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvujfkfw.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gqginzfrw.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzcsnjtsg.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdajmsokm.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/guhatnmcd.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gobiltmcg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpccfpwaj.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gudxzhpgv.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glryivzkr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjpcdixj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmzfkzeh.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkhifjenf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/girrbsyaz.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gftbixwvs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgjweisi.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gclkypfam.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gytagvrau.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohhxhown.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqqjxlfbz.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gzltsvrzu.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gdcekvcfi.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/glgystdxk.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gjbnnwvfg.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwpuccmm.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/goxcsudmm.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goynivmis.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/golexuiid.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/grqgtyjhb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gncasdxle.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdpslxet.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gndvlhwsk.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdcgtgnv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gctelpfnw.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdedctntb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gethvngxf.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gshmpiobw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyxhzbww.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpryptfpu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gevhhozak.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfmukwmw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmkbqmuu.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gajhtrmyl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyasthyfq.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdwtguan.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtcxhlval.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gezqhroum.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuzqryzs.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbizgtnsg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxipxtwkp.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgcnqksd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gykpfmyis.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gdcwoavzq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwiaulhz.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghcihbych.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gmyzwrgrm.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnfcidkh.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrflrzvd.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gxxxodcpg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbjldple.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiqqpiat.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givthxtoz.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gszbtprdw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaazghws.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcclyodf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/glibdipso.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ghyjqqfwu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glksogpdu.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gyupcatwt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ggpwlicnj.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkydixgy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdikfqoqh.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcmadqhw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdbiqwnd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqmjwwpe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwvtaapy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gajivnlvu.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgirkhar.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gnnuhlled.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gduobakxq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gjcifbagq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggebhvawk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkozsar.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/ggdhozxvb.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmohrcvjh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ghrsmvsub.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmdokzmc.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geqqkbxar.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaxpknzw.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/glxlvktnq.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gthvjvune.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhftienw.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcnadzan.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyooiqtj.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gqoecyjra.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gczkchgov.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqejogrk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdvhdlihq.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaucgesyl.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwjdhhqhs.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gafnhhwxm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gdorstgjw.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gafbslexl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggubiltzd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhohbsnc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gdpqhdbih.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/giraznpck.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqnyjuzm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/ghbnqaubu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gvmzhgzsy.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnwjmwmer.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlyryzha.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsovqlerq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfugnltm.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gryxzqhng.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gkgqdqftd.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/ggpagpaet.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbhbvawd.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzgxnbkz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnxiijhy.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ggwawzool.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gpsqxbdiy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbjybgxiz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gducdsrtm.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gqmlshhlu.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/godgbuevx.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpwbpvxdk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkffbgti.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpgyxbmwg.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuozrqpm.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gzqadsjni.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzykatdon.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/geznsqxdb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gwboosteh.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/grugpbxoc.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gocnzglsi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxocowjah.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gefylxjdu.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfqlumow.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghykfdjqg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmpoaleh.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gidvixbxl.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgcxdsgc.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gewtkweyu.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnhgchvoe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gjjafzvpw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtldmxdsn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnrbpdmql.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcfytlym.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/glowlnuib.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqtcimeb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/goltzpsyu.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gguwpojhn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejddixok.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/giigtgdxr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrtmxocd.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gaeqytkzx.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbnswfqg.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjihosne.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvogwnerm.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gtutvacxp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gszjssipm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjodnddj.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjontawv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpeghnxe.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnepdbbdd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvzhlimq.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gksqnaniz.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gkobjzqgi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvccnkgtx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwsxofxy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnjncciw.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnubakcdp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghngtwqob.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmncmqen.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpewghrv.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/guhxfnshb.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gotmttkiz.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzbrklkf.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gzoguccoq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkfbnhxb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gfqgvuglk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkrgyxuo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/godgvpagk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzwerrwq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelgsjcsv.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/geqkzuefz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlnnwmot.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gztlfpefv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghitnpkyi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/geobomjgx.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ginihhken.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnxkvomfc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqwzusus.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gooqshtjh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gilolzdlk.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gjpzqbkkw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/glfooscni.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giljgtawn.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gyveohyju.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gablsckba.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjmextso.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvxydwxw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkblldos.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gecxpzunj.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gcbumrgxb.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gckdcpisz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzdtwbdh.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxjlruor.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbhmeahb.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsbzmxro.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahsupxgv.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqvdeynv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/geqdkpqqt.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/ggofwdbzm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/grmxjsdsc.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gaovakmzw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpiokoww.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnarkhkqb.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gtyualeol.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgbdorip.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/grcrvqhpd.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/geykxleov.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgwyetj.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnboewyzn.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gsyljsurk.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwlbuuzm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gcqpgctel.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmocizh.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqotvhqvn.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrdiocmx.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/grulrhstk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqdmzebh.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjiiblyc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpomgoqwf.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grreolwcm.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gqehlrgxb.sHtML


<!-- 参考信息 -->