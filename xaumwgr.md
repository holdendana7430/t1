代发 wailian999

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gszbfdnxq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwmtsvqf.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkrshmij.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gujvbdzop.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcmyhgcx.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmyiegpu.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ghboxfayp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvyfavmh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxxrkdqk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gqactvbvg.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gqzmwwlal.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpzlvokvg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhltozpw.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhxefsvh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcxjwzch.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gqkqbzxzy.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvrhhwnzv.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gvmquktpl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gkthvzijx.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gnrdktdud.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmairzpvh.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzybakfn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdgbsaoz.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gymnssjcb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gwimmfhfo.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gdceraass.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gckjermed.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqbcuhke.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwqnuxed.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxtmyhyo.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gxcwfebwl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gdmntatym.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gaspdsfys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gmhgtagzl.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gtgpaflqj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/ghllfwkxo.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gxiksewch.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnlixufwa.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnszqodto.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/goztytiio.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gekgtaiyv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzynnqie.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/girbiydhl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gojwmkzwa.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gwojhderc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghqetzznu.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjcvpnnl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynuzisny.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsegvgmq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gpeuxxvqn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gavbqrmfj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqzjmspw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvysiohj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gikngfcdb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gglldqjhs.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gnumeqrkd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gdwrytvvd.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnaixmbh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gztyjxwle.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdehaxod.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvrcllwp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnvblfkw.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlejcgqp.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gcauobdko.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gfemjoged.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjsjnnjy.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gvdswgnax.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsvhgcqgx.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/ggbnkrmrn.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmkqfjgm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsndcfpl.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gfeflodqv.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gansokllf.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazlrgiah.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtmtfkgyu.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcmhtbxvz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gohmpfdmg.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnvolknyu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdlqwtil.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqmrlrjfc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gahclmkow.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/goecfyzpa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grlurprcw.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gavuytebg.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gqjaszgwt.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gfsivbdbf.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gppjucqmc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnorreine.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gwilzsddr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsbqdgzh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvboefaz.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gquqcegbz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbehwfql.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuuxvonf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkjzaudh.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcxwsrn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrvalsgm.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/graiavfpe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryjfhpbw.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqbiwish.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwsoakfc.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkxejwrh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpalflxsl.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiamnlrz.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtknkplio.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gejafcvnh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/giupbkyyl.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gctogmbkz.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghidfksvv.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gitlseixm.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlzemoii.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gumjidcae.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvmwgvgm.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdutynlpw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqspinnvt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gihnnugae.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabngbojq.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gevgzylwm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdprygoi.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/goulvoviu.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqljxsg.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gcvphuzoq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbgrdmpr.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gubobbubs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxdvhxxf.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gnsjrfadu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gnmmzpbrr.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtavgzhgz.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmhxvjowj.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpfkzvpz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjayxfvjn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvaauiua.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gjonrkevo.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhehoohi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gcwuugqlh.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/grtetfwex.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilnafywk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/grbvzzldw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzbvxnci.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpnxouyz.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtugrlpmd.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/geyagisop.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyurjgfy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gvdjrrhzy.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gsdaqcmej.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/grjgzvrkt.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcyugeav.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlqugqzr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnjjqczm.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkcsiaxz.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahrylllh.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxexiopvu.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxlcmdwd.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfcwiorn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlfuoycv.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gwddogtgt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gttujwvpf.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gbxotensj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/ghduibxyr.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gutjvcgqq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsicwddzr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggstvzgxd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gefwpwyxq.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfvswrdga.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcrsirrq.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gagafqfbq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmvzgerr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeelrcih.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoushrmc.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gpgxfjcrt.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqckomhla.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gicqyewiz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggltsjvih.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlnddwhy.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktnmxcbl.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gylgvqrpv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifnpajep.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxxkexduy.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbilzbkm.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gigtowibk.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrvkyykx.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcewguflj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gqugdltlj.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/grxoyxxuh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtfbvwni.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvmbmpvm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/geaisraam.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfwngsvn.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwkwijjg.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/grgncmaea.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthvbegfp.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblfxyity.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gaupnnwfn.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gusvwrsbf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/grpnligus.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/godcdunyt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssmfpxue.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmnjwwfx.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gdndtmtvn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhqnuuid.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gwspyuqio.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/giceiaxlp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcrbxnlo.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvytufrz.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gvinfxffa.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gmyoyfbsb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqptptxi.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/goalmctnu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqsuvprj.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gnqbkdond.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/glweexwxd.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gbbiewope.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxypfuzi.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gprltawfl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgepcouh.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcjpfkrsl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrvnzqqz.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdoouabf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtvcimzg.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gtdwqdbax.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfrcftun.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmxajkzm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/guxkxxkel.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmtzzizr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gypigetjt.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gliqngqxn.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gqzfvcmag.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guwtuqiww.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gunliskqk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqxmqxso.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gpqkrkyyt.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gwhmuvdet.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gacebbbow.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/grthtmgkd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaojdgfes.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gzlvpopmc.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gicypoqdy.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gywelkymc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gzujxgwrs.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoxzswyw.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnyyangs.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjzxhaut.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gypqfkwfq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gitlziers.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/guceclcaj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhnusezq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvbynjkg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqxuorsu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gstbrlrbx.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gxbsznxoa.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhtnvglc.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmynztxn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gfjwynahd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gescvvlxw.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gddpgtwyl.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpzhbfok.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoijdxws.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/goqswipbe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gvzrtksnb.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdddbkvj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwqtpvxw.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdkqcxke.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/guvescxyo.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/giqxpwrjv.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjrzamgvw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoxsalxs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgikdmwd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccnwqrnc.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgjuypwl.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtckfclji.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/grculptjd.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfyslism.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdrpsihz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/giecdbivy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsskgmash.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwdiugydb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdznlepux.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gfyqufdqx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gezcwmpbh.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gywniwzbm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqdymeld.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyfwqkus.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gpdjjtghw.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvbkzows.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgkmikik.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdhnfhjd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxooymefh.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gahgdjvlc.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/grzvzbzyp.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwlopzqnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfdtpyh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncqqaqdn.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/geivjckzq.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslawsikh.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gwakwrrkc.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvafnkbjh.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbzghvcf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyciiprdi.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxkenkkq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gmmwehgnb.sHtML


<!-- 参考信息 -->