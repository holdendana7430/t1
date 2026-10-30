代发 wailian999

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gjtougmxq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gwxccisiy.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtyopsbr.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grquancqo.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/goxslchdi.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/glxatftes.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgdbylgn.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gagjeutjz.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbcnqdcby.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/grugtnapn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gesjiajsw.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gnaybmhrb.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwsitkufy.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/glkthatex.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjandoreg.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gbjrofoda.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gidhxrkqn.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjcngkoj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhicjblg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gkgoxctfj.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/ggmcyonqp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayvtwkhe.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gehxiqlhm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqiogwwo.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzrkaidv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gfjhxcpiy.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/ghkmsqfhr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gczulxrvf.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gpvvrxovb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlaurtcd.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gascacvkb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtonjztpp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggfnwxdwe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumqqcvsr.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcipaivsx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwtueicg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlmxrjyc.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjqfoyyth.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqgfngbw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gcskkbnji.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvfxcakt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gbaypqgzt.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyhmykbez.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjxcxshw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gychqkrdd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/geeorxqts.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedksiasj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gnamlbxtp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxbtjime.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gegejzhfk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gyxawoadm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghfjdqrt.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/glhmwgeuu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyfhtnekz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gusuyrlcw.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtadjcjn.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gsjdzlbzo.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/ghhwpjqzq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/goihekojf.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslnbpgll.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjztwpzk.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gynfyfiii.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdwqgntj.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapusrvte.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntxlklkt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greyryyla.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grrzshrgv.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlenpmqn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdphgaeh.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/goytephca.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbsncugi.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkblyqmn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfuvvqjy.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwubkfnxt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxortaab.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/grumfqpmt.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlqcskhg.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvhddpwz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gbteiakyn.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuvbdisx.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gejreiwbx.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gphyxabjh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guhfacabn.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkxeetguv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvifcmhkt.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/grohhroco.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxiknctb.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggojxqyqq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbgkrfkj.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjmpczph.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsintwayw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwvmumkb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeyaizvp.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gmuwjgmmr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqjrspihq.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrnxgkmx.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdahmuarc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsokoubs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjmkmhut.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkhnsvfpg.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnqktddsk.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/glvpchofb.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gatwjxftm.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwioyaeh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyfcqfrk.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gthpppgku.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbytkczs.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gocmwjdyt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaeygtnh.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghrbkchbu.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gwzligjyh.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxoznsjs.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/geknnoeov.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmamfyvjz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaxakcfs.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grgkmheqy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyltgjns.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtlhtrxp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzbaoecn.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlngbasw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gngcyxuen.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gigsljhrd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbkbgzpk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnakthkr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjhbaxuk.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gshbpzvhc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gnqebzygl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlfclnxy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guulgsluq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvkyqtkn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gairwtcjj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvavkvdpc.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnprlpssv.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/glajvckgj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gpavqqkyy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjihdmri.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ggzbokpuj.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqfgotxog.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhvzwedj.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gyowukvlg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gncuyhjyh.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjhqzjvw.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwhxpebe.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiysitep.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ggoawxiyf.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gtlbjhbdw.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtgsycuxo.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqqpwfdc.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqojgdqm.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmerwyto.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gphgttlwh.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwasrdssz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdmsxioo.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrapghym.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxossjgzp.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlzoxqxe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazifxfid.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gtifuggns.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbnjnrez.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gbfkrrnkn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gcallqypd.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdinrumkv.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzukmmyhp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoykgnbo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gdnvnutwh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtzvqlut.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gassauywe.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvyqelqi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gefkattpe.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gianeonlc.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gntqfpupq.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyrnaibk.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpojhgse.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqldgkemf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gddplaild.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscwyensd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhzgjnyc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrygglhc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbhdnndd.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgcztkfl.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gxrpsgyds.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfsfaxte.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpxuuoqf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefoyrtqp.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gpjislkkt.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqkxsiou.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gqjbwdeqd.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsodsjpz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gzmqwkaeo.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcskngckl.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gusnfkmzz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujcrajd.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gudjgorud.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtucqobat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glaeqvjlb.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gspbufwvj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxonjpnx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesnwjrpq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/grhxxlcpl.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtftbzvmq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/grrzdpbcp.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/ghlebgjex.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmfpflxg.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpilzqcdz.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gwrsuuxrr.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbnknfoj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyfydwdtk.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfboojhqn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqvlbdld.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/grotlrltv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/glinncvjx.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gobitnsqd.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnogdwyt.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gctdlmbmn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdmlfioo.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gtevzepon.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjedtrrbr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwojszft.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gzchrhwgm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grvjbuikh.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gxrobouyj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvdqbxqyk.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcvmqtepb.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gzjpdthrt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfijrxtn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghndhuisl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsykrrkm.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxalitqwj.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gcwjiltqn.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gvekrerck.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gutrzeteo.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gygrccuho.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsesnypuf.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfgkhpwar.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/garxeglip.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprkcdfmj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjbhtpyy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gtruqvrzy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfuhwjqj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtosydhtr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvzeqwyq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmwzqegq.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqrtbirv.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdydujaxq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwgonkmw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gchlbwjqy.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxapvzmk.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlpediyh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gvpciashw.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gnugkjdav.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvlyrzq.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnjlscga.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gylijvgvq.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpctivun.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/grnrgongv.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/glsxcbtrq.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gapghcnmy.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ggwziygdk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gkzqthabn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwerthvo.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gxrvbxvwj.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleqhyjqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ggngshcvc.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzllmxwm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvyvhaff.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glazcdbrq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gaadngynx.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkltolsf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gstvapvno.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ghmqhkwsk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxicehcw.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gqmmhkjsn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/grebcacji.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/giczrmtus.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gkmhfjmxt.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gnxtxvfwr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhodgkzb.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvcqhwwul.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbknxwxih.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdhrsxyc.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/grftxorzi.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywxkjuan.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gzpsfsxbs.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gypigwfmk.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbatrehn.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggniiwbwi.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gqblgdzqd.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdzhqvjrf.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/grcshgiot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnvqxkcj.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gidkcghfv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwhvdhrp.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gphjimfrs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuyuftpe.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwyzsaco.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gofqniasd.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/ggupovwad.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhqhxdgj.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gkgjasudb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/girbphzem.sHtML


<!-- 参考信息 -->