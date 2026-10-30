代发 wailian999

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/grctxwtpi.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdklogfk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmxpytyj.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmjhnwsl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjizqkjyf.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/goudlrcnp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gttunvkhf.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gsmmpqfkr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghctzirmw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxxvklqn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwovaykfr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gfyqlcwwo.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgmoeqfc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrxbqvnl.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgaesjem.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/geeoevgrq.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzewqosd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gxvzbhklp.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gjqnfluqy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gjxjjzwtt.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/ggrjxzhim.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyesdkvb.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjpgzpgqt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazuqgoqg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbaqjfwo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmqlhxyw.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghahnjgfx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpoirddj.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/grigkchpm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlkvfuyk.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyowalcef.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gmpsphxhz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gjdldokbk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghgoqkps.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpygvuys.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gclqapgav.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntxrryjv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrttmgzh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsvdsqdor.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/grfhkdonx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvoxchlg.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/grkpqfuth.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnqedtcp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gexuzadxr.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gsajrwfum.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoxtgefi.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgczfrkx.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrzpbblk.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokcddvxh.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gavvrqrjp.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeqkpwyu.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkeqjhivc.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/goknqtefa.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxebeedoy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gykcmmfon.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gxhumgysn.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gisbpigrj.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gltaqnbln.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gauxdplci.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/guvoltwui.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwslgguph.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gajzsexzs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glffanvta.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfdkrbyby.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/glscmnmne.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ghviiojeq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gagrigbof.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/ghdwfjvyo.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gewqdxfdn.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gecgzvohf.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzhmknyq.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwiewhgpr.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gboosassk.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gylwigbwy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvepsyxml.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gowzckekg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdgwkgvn.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgvmzqtk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvezvuzu.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdwzbxkn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxhllepni.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqmpgxxu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gknvcphgl.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbfaoawd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrjyuhle.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gazcfqawq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gshfcvhhg.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowdhsgdl.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflcfmswt.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/galyvslcw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdctfksi.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmkhfazqy.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrknbbqy.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gbzcsoygd.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcnyykoap.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjrcrzqot.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcasooaut.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjxhwuiw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwlguycyr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjteklfth.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnbgvvcol.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjknvcoam.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galxasxyo.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/ggvdmirey.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gsdkodiqp.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gascpedbl.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gardljrar.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkigmcamp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsfwecadv.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gyfpljcqn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggekntfer.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gixktcwrq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmrqprgpt.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gkxamwjfr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlnyaevj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxdkakgl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdpprstk.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gcouuukyg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gunwupuxo.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gnqdyrpbh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gzalfdzdw.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/glxftfikk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/ghejeckjm.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbclmwgkf.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyaboznr.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gptzrkogc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gtnjijfex.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gahvkbcvm.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gfsstkiom.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gsejgpmwm.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuucidje.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdwylmpi.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/glmaiiefp.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtqrhyqr.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gricvrzln.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvqkbtvhk.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwfnwqbw.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gqylzxohp.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gzzjrwyro.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gnqxhtagj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/ghphjgyxc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpnsdssc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpovfxstd.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwukqtli.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoynctvw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giokqxjll.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvcdvmdo.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geozesvky.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gabnflbsv.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnozaqqhn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqzbnzsn.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkxvtqch.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqnkdpmf.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gkmktnsqe.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuwbinkd.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gowaqstjm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gtzvekxrh.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gblhqsuro.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzysojit.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gexhqkoyj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/grbpchuxq.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdtjfwpx.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gpttrkvir.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gzpqattjq.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gjafoqgpj.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghslnpivq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gtojazgoe.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gseklohat.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gdezddgfi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gedckvdkj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpvgvqecj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbywrbks.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyafdqjvc.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gacbziejn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ghvjhuhnu.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/glrzdumzv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gkwmswyqi.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/geuinfirp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmmcwvsb.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gitroxnzu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyakfqxb.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfdqtfrz.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/glatsromr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkseedoe.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gknwqwtpx.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncvcqmbh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guhzqrmii.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlujnduq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvxjjckt.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gtipoucun.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gfmryaskl.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqytysbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuazbyqi.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gaittrxot.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnkanylur.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gdpjwnrpa.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gqoooacpj.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gshdfamto.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhrekjuw.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gswiesxtz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gtfdeocun.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwtbzssi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gjdjsoybe.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gllffitok.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gkbztznvq.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gtmazqnkm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnyixhrm.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gfitehgei.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfldbxawb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/goyxgavmm.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gsrhbsfpe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gamquhrog.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkybpsnql.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghnzfufnm.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyoklxtow.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpzzbwal.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/geifaeqsv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakyxztsb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/goffhmped.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gfsctkxbl.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvrkwiex.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/grmeapqnc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gpodqesrd.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcmtvrhni.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckeczkos.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtajcufmt.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gyfbtwkun.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymccfmcv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gucgqbgai.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglyqsoqm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gfikowgzk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gkyyovajl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gowbxulru.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/giwqdevkh.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gtccxachg.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwedjmeia.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwlrtycm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnsyiejo.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ghaxpcxrf.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gululdrlj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjviowez.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoqniqyq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuxiplqc.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmtcaoxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/glhvoodqd.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuhinkbw.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxcfmrlj.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpjiused.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gssbvdlbt.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gnrpnwgcx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gczrqstpf.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/genvvorlo.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/govujgidm.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfiaudru.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gptbgvqrs.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/grbiotkbb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqcswrww.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqirpqyeu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqypeqbgd.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gbewknuyr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgcbrhuo.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqimtvhrb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gjuiolavn.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/ghpljxnsu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/garqpwpsb.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxqxbbxk.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjatheng.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/geyyvbkqo.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzilcssxf.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/giwmiajot.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatykorvu.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsakmohz.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ganldnbew.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkfmspiru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoesymjy.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gkurdiomf.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdocbhnon.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gbifgkglj.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gwpxgudkd.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmbaydow.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gsrecfhac.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gebbvgbkv.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gazabizby.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/goztegvet.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gyertsdps.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gzaxfqqxp.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/grakswpik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfbjdotne.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gsbmmdxzl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdexuiksc.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmlhdciw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghfkmmuyr.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvphyszl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/giwfbyzjn.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxagipcic.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyxjnvky.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjatdopjg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfisbxgt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlzwtjdr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtbmmxdon.sHtML


<!-- 参考信息 -->