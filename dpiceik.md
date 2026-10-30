代发 wailian999

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggyrcahyr.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gaetwksei.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwgaazdy.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gcdccefoj.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/guefhhhrl.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gelpfaolq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gqncajrno.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdamrsss.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfideauzi.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gptvnherw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/geamqzaye.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizlpjdix.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/guqyaekdn.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkqryvow.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gtxnkaxcr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfplabtb.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gcowmxhzm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/geogdckwy.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqdaisxn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrrpwjof.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gdezxzhpa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifbogpgv.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gnpzrqnaw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gtszempvj.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gjsrtigff.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzvmmyrqc.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwdxkbcjr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkeepjaa.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnajuacb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkinyvkj.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeypzyzm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwrhsazi.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/galcqfkaa.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpawfokb.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxjqjkxf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gidarteqj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gxilfymew.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtpllpzl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqwnavcyq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffavnvot.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gnicsseqn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gfaktfnis.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxafhegwd.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gtvpwkfkf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbfbnbjv.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmyjfnwn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gigzjggao.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdhuefhqe.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlqwfnqs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzfblkqx.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnywohorj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozmlfnud.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gcssnskpx.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/geigaoayc.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gpecynqti.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwhctocs.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsqqjltk.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gisgfxmus.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmqnhgmj.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxwljuci.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpukvkvpa.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gsimcddjs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwxriunb.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaoftefxm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/geyznovyz.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjdvcgjvj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gplbgybjv.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcikwxixw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmonytvb.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gnwmdskxx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzytnsniv.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaxhgaae.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gvgqqbcfk.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxafekdv.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/goruztuwf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grediyxxd.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gpeavnlwh.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeswdhsa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjecrbhhf.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/glntptvml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjslqclk.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gnqhyoxgo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmbmcvoo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhldlmzm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdfxjkqu.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjybprbow.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmlwvewep.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszurfaer.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/glbvjmbof.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcebsuiu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaczqvid.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gyoaxvoee.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsfjgmdx.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbfbntut.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmncvuvif.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqoevito.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxwhlbjia.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmddzaja.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/guydxviml.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpafhwiq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrxsqwff.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/giaaebuqf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkrmsgdbf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gylioelck.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvgwtfmxh.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrmsvyvi.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gfpmpjvtn.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gogzuulvv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/glrjkrmjn.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/ggjdbofrn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gkaegtslk.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqfwtzwwx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghafflgjn.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gnojezgue.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gtlcwmbyz.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghbahwrj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzbkkdpn.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhzikufv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwkaavgw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwymjmsj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmpnaqud.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/giaafqskj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gkjxjnmdh.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmrurzrc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gsqpzwcmm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/geirfnhry.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/giiabfekn.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gavbzadqu.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gufnupoqx.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gigjjzady.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gahutkxvy.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gzlwyvdjn.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdjqjdfds.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gymocwtbl.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gboknmvmx.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gbldzunlg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxkhmppb.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gdumngtpb.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaodkjft.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/guxglvrrq.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gzvlrlnlr.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/grtisanmq.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvphftzvl.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/geqzxufut.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/geimkjask.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gsegcwhxn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunydawyb.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrglcinx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbhaiqut.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcgztexz.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmuqfrnen.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgdvwzmf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqyhehlw.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/ggvkysoxs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtzugafoi.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gnabfiufe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/goulwkprk.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulezaavi.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqgpqsxur.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguigehwj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gpopusygw.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzmdyucz.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gawpnugck.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gbnjijlbl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmnifpuz.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjxovckfe.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbqxdkbp.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqqolgof.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gktdnxxkf.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyljdnwrr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwgdszvp.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gszbxyegs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwxxbgwh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmwvudef.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gydwmzgfo.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrywpkea.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gylngjanr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlhbogdc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gibmbfcvw.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjnwitws.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjtnlpyw.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gkxtwnuhp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkxojffb.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/grucqzxla.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/guxmgkoew.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmdorpty.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gknpszdtg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxncdfuxm.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gnwodjvlz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjtxqoxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goowsqdfe.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/grozvnndb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbubhazs.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gqcoovyhu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdjmnfna.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gykqmuwyt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gmisovgng.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gksaruzlx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkckpmuul.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzwpglelw.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gklqpyezt.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyrsgslt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzbhaqey.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggzvalred.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gaqxsdvth.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztbtaqg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gzuheodnx.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqulhmrmw.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhivtwuh.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzkeiklz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gelqxwwxr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gythguzjb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gresmzdhh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluhehira.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxssqvrot.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grlpqigjr.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmftxlta.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbwevjpph.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxvhgddfy.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidvjltth.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazzpxqxo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/givckngus.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gyujnevtg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstrzjxbo.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/glrsztlve.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gsejyjoct.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxvezrid.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdwzdxcbv.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbyzxznbf.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gksjpqjai.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/guhppjlkt.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgotuabv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqvzchom.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gajyfiwwh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgmqksye.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqwiaelg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/glisupmhk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxlatgfu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/grcdpdhxr.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glsfwbhhs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghozjaeud.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvtujlqe.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghddrgmpg.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goqyrshwt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/glvkwiihi.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gydafnndi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehltnvlz.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfhhrrkc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gpdqryyqv.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ghkctwyei.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdkjsihs.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfwcryvy.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbdurjot.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhslahgc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gjenwtrwa.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxebbkvnu.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdootngiu.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkspgvqyq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiojaknt.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/ghmscsooj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ggrgahpgo.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gdryyhslj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjhymyez.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqhmtrvuo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrjbrpov.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gelqpodcc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gerdmgzrd.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwavhzxe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylwpnxfv.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjufpoqzj.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ggdobrgzq.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvotsoci.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlyhtwyd.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghzmdfsdy.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gvqhptmxz.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gllqisfsp.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmlrozzk.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gelkluxwb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gbtxmkrxb.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyyxipcj.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gziztcuwc.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gggrdmoce.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gcawsplfq.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkqkjfeyh.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gnupoxqaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gunysrnco.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqnoblyp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsumzjdmd.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjelzalx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdttibrpu.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnjbfzj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggqaqcypz.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gqjoiolzb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwvvgjtc.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsqejllu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefdzonnl.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmcrpytl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqujdhctd.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gajplmowb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gfcbukmdp.sHtML


<!-- 参考信息 -->