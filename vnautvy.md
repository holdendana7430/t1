代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhizknfd.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpwjrrjcq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griemjbnd.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gwruczqpm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gubxqgngu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gbjyyjdot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gtxqgfbnn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxxfqqhfk.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqmsiuaa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwywbipvm.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgffdbcq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gqfzmaxax.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gyfzsegvr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gfiwbzprg.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltmuytda.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaojjjsc.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gsyincwcf.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gdsrnehaq.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gubrsszgl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gbjhbesqv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsfqptci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gmkghsosv.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gcranjdur.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gybarlhtx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfxwrqif.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzclqhuy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gctyrehet.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhueoouy.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtromwuau.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gxhpfahpi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gesmgyijg.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gwhuayftz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqhjyctj.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/glixzzqwj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/goubougfp.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gykmwabox.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gvfdifiqy.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gprqufyvu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnqtloib.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjevayfgf.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/ghulvsiap.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjowvnog.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gcfphekiw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/golurdjab.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulqqdbqx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwavbcfac.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gkaddbvbc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gojalkpch.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokwtmzsn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gahttowxd.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/golqeeybk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcybkogrg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcduoymy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gusianxga.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthhfnshh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqnbptiaa.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/grgrteigj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfijyoap.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gkakxtuup.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfbtotwn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gbmsqoafs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gqohtzjxh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbggconca.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbibryvfv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzusenkd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gyypuozhz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guscxdldz.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gssurrwpr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbnytijm.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/goiipafyb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/glgexufay.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gienqetea.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvsrtqtf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grnhbtxed.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gbzshrmjv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimgzecyj.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gqmlinunc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpcyywbq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvhgfwdo.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gttffxbkb.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/grvlmqsri.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gnxojuwdw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqmsrynv.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gekoiyfhj.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/glnwlpcok.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gfwlopqie.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqtppwul.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrtyampz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gidxykxxr.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdchsdxwy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggwiytbuw.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/govpbqscx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gyletudmg.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gdryuvcut.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqyybllyi.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqfxjajk.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksvtvpbm.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxvopqvz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gevtnbdhi.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gimqeynry.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gnibmtwpo.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gogefsdor.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixfnhfsg.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/ghpncgmqq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gusjsedgz.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gtzlaiyrp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gixslworc.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpwfudsax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrgthbbg.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeyixtvy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvthbmkpc.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/grughakmt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrzrmleu.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwnkkahk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkrdqkym.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtvvnjhk.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkvxryesa.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gbygtkani.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzyebuelw.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhaelmkb.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbqvdqbcn.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlhoaugj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grioootyb.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghotfmavx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gejadnjdd.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzigjumla.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjdagbchw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqwlbzwp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjkrjyme.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcbgyvpx.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzfgkleh.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gcmwqzegw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gpvakiscp.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/guwhyomrz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkcectub.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyacgurfw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcmcgpdu.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcpcpbwkk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoqbzaog.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbacjhoid.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grfodjvwt.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvjztbpg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtonvdwxk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gvszxlfgg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqpyuosho.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gviinrgyu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjyqoxxv.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcrbpegd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvetocku.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gujsyxbew.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gsduroozg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpwbkabto.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzbenohfs.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gujjecvjy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/ghdnljbnh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/ghnctvgar.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ghgukudun.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvizqjqhk.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ggknhfesw.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbarwbdb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gsauqbhgu.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gqroicwua.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpprqadwd.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsvaffwow.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/grfvnpsft.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/grujfrebt.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/grrwxhfsg.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gwysvduan.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfrnzoqp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmydcrml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpbhnfhc.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gihdqgrwe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvchqrspk.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/grkvafkjy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxyllpaca.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtdwdbfji.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/ghppfvfne.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gkvjtcjab.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gziukasen.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gkyhxfegs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gpieqktyz.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/grjmgylff.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyczwgval.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gicohihab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gpsghulsq.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjylxgsbt.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkcisdmii.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gzakeaaeo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqexmbii.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnuqorbpj.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gatnyiqyq.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwqtnedj.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gkqwmfple.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxvlxwtq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrvafasv.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gosnrqlma.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gynnmbyde.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/guahzjdvo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvmojbwt.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gryaicard.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gevduswiy.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfhakvsfc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxoodwft.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gydyrosuq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gxpzonhol.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqddvneq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkxqnpca.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjersrsn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/ghcfdjxve.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gqflmrfzj.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgdfksnh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gttrqmwrj.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gvabzowmy.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gjrdjckox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhwejcnd.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gahvgvnjt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/glpsyumzb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gikkdxunx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjvezerv.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqffhqnfg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjkvijmz.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gatjerxfl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnxfestjc.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpabsxnbo.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/groirjalp.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gkljdorgt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbwfkqfah.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gppgetibz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjxrqegm.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaekyowqc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ghuyckfmh.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gpifjopwq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuppeknr.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdpxjggz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuxgofyd.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/glxncziog.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwlnhzbdw.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsybfana.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gphmpnlpv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkihrnssd.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gokrwqvli.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbpdzkiv.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvpndohxf.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtridiggi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfjnzolky.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gghugjmxt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjgwgdvp.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggppjnmzd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggondoxor.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ggcugitxi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gbimdupsc.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkatbjtwv.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyixvryss.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcpzbbiql.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitrzmeiw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gtadxnstk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlwdcyrl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxlokyah.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/guvzqaasf.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpiwpyqu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbckyuji.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqlxlmje.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gmylpuqja.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdbeesvlm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/glqwldzvy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gihmrebbo.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gajpbeidt.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ganmidwpm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gmxkgxern.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglblzynx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmqtsnqt.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gupfavauf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/geojhgddx.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjyilswg.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/glvnobikq.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gyyafvflk.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcltvpypy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghipfhgif.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gfpyergqb.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrcfuafx.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbzwvzbm.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxftvteyq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/govydqxen.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtugunije.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkwkjtai.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gmdpgomad.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjlnalvq.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqaywvupz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/grukfkuwt.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gohurxamw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatfpcokm.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbolwkqua.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwaqbahr.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnscppjzl.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gjttpiuce.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gitzckbnx.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfpcmdrw.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmbccfom.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrlcnqnr.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkbxhszt.sHtML


<!-- 参考信息 -->