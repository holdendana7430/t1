代发 wailian999

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gxzihmxri.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkiccpix.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gkorabhsh.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giprgzfnt.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpkwhuff.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmxeqgml.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gpkixkuoj.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gkqpvpxch.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gizivvivx.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/guqafigrp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gsddvvbpp.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gzxtfhyba.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfntjucgf.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhbfjvxa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/ghgjglzpi.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gealstyng.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gimpeeqwj.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtwfhmuyg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtclnwcje.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gvgmojuip.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/grnlorylb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gtadxcwfk.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gshhfpkpe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqzebogl.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/glpvjhmqe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gbflopqjs.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gpezjbyxl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gktkcncah.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gexzqpicj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gseqwedur.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjwpjrsj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuiqovsz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gepepimve.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gljgwyern.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdeukvqc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyskjineh.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gyilozkly.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbtzafycl.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gkznaimaz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gycjlyoqg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjyzrmyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbiagihd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvutbrhhz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxmpteja.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/giowxnxjv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaaqvhfx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gokkypqnl.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gnitzqnna.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ghwzkjmjz.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoyyeqcp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gbprpnsyi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnfxxbhl.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxxbfly.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmhvsuia.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugreidhk.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gptfrkcvb.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gobkezdxq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqegvixr.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/glvrmkmgk.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gigiwpojl.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gckvsohxz.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtycnssn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gknrjjiyd.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gsajwzape.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaxpidto.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/glemonxgm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gztnawfoe.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnsoktoyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehmetmbm.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghrdjobir.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gznoqeqmx.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gflrcdhre.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gvbeedqgo.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaoghzmr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmsrunak.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gmnyiiflp.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/glncuerji.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/glzxqtxpo.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxkgmlfeb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gsukplwru.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/guslnqstz.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmmiqwnl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gupznjxij.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtwziqswo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyanidanx.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gazanirzd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmymxygu.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gweagrzol.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcfhjryi.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkusrhkgx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhqhkapa.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gqznsxzdp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gklaqrxwe.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gybnqpbrg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goleqhtrs.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gslzxkxav.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/glsnhlpey.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgwznrjg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdsiwzfcn.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjscxhnsj.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnycnamxd.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbmgspfb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gougcbenf.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gffhopton.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzphrtdds.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gevbokoif.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggymmgfqz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gaggecdov.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgqzymiq.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghjjfrxzs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfumbvxgx.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbplxextl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gybolteip.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gtittzlgk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpzhpfmk.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqijxkpvv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfglqoyu.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gwmffvoyc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwlimpcx.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgdiqswg.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqcnsrmj.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqgnvjuy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpijdrtua.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gvhxhpisc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/glvgmmhvh.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gvouodaqr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gyfekfjlw.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gfspormet.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtcxnnuo.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqlykeqei.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gubgzpiin.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzctfbbxz.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxiehsoz.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gmrpudypi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyoieayb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gkxxverci.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/giikxjauy.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwceceeqb.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlwymfaf.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvyxasrym.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/grtlgbtzl.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gafuykhnh.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiezrslg.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhzyslx.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbgfmdr.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gojnifjkv.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gvxplkxnd.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhspowex.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjdvhawd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gldtpytoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gpyiqtolr.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwzrosgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gduzgzhtb.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gagoilydy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqprrtazq.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gidxvplsx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpyhgvky.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvmserdvb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmhhcjblj.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdxsxfhy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/glrxzaajd.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkfnvybb.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gacebvsnc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gckzxsgxc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gspzhmdit.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcunhxiy.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gimbchhgq.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwdadrfg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrnemioc.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpmtswyk.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgzfckhj.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleqxjmry.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxtzksax.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godxcfosk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadwqbswc.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/goggpsfxz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbqbrukve.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gwtkimmpl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gifegyasa.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gnobdrjjo.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwidoxgdf.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcsjcsvzb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gewbuolrq.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqorjijcn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjlezwzd.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gmjfpwrxb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdfocfkk.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gycxnrdcm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/ginrobzek.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrwtsucc.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/goqfhntlz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gmxlorcko.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiimdvbu.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gcnsxgqla.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gszrtoyoh.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbvgdhjb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxborsba.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfqeglpl.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gatcyrlun.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gzxnizqgn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbesahlbe.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gapfgaogx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuaaztcs.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/grciitsel.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsenpmjem.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxonbbfh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwkwnbbiq.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvgbjnzh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/glqyqrpbi.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gemmqjctu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gqcgywsjt.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmxukqpn.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpodczeo.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaxdxzcx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqvkgsxls.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gjabyvwbm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/geacdgvry.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmdeimse.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyofcuzbw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsjiiccs.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgzwjrey.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkeoebvw.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grgjvafhz.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gwppogjfa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghiwzhrfr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gppjbroel.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gpfeqbkwa.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gmmlpzdwk.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxavdthl.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/glveozspw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudxckfix.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghncqtsan.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyghxluv.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtrejohek.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gbomfjuqh.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghrdirncz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihvokvrj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gfzdthlrh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gqfwawjkt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmupcklsf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gyeqiseqr.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpbhlkqb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gksfqqwja.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvyrgqdag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/goehgylry.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdrbahwh.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gpyvijpqj.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghbalwwqj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gdxpnjvxz.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gxgxrfhzn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gxpjgozfr.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ggyjqtubc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/glipobwiz.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbksmiql.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlnawjnd.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/glntqefvr.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyivjosgy.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/guvjkaqxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/goztmlfhb.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxtghjcf.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gyoowjhmv.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjcdbfio.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/glfhukfwy.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gjshyslsd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnxphxet.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gxzhfpgiq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdnuvnfm.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/glxsklxyd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gicpxmkun.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gvbmgzowp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ghefhrgmf.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gwydfrzrt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/glypkprcc.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlvrwlgd.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkobvkgf.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsjznvuj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjztlloha.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdhflevd.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gbbeunlnl.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvxfmarp.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gwhxrdsqw.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnmhbiad.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gdmlgmsmv.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjydulkvb.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ghjhvshqa.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxnhrysb.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrqcysea.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gijtrrrth.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gltcczzez.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuwggnjc.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrmuqxzf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gptjgzhsi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/giygetfzg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/giaogzuqi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/givgdsmiy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbubovqdt.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhsmrxrk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzdlvkrm.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gacdjeueh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqanziq.sHtML


<!-- 参考信息 -->