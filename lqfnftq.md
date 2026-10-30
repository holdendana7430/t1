代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnxeyjpm.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkxbudpv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gfiuybuvn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gqdburbrs.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gcepgtjjm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gheiteyiz.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gqwmadqmd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gpurqwzfc.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/glhtkpiyc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gmijepniq.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gydmulque.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/glbjwtdak.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gqzvomhlv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbednjwi.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfexrpooj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgmjzanu.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/ginyamzzg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmszdbdc.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gffonxhos.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjzmroaf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbskstvri.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmleynfpw.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqmooeho.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gayonwpeu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gjypimfwa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gmtrbfgub.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwparqcbk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gmmfzuiuk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gykyvwlve.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaahaxlm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giocuqfvw.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gbppstiyn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyuxvgno.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/ggngrxwcj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvjyzvzu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghpoozksd.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuyrhnze.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkbwwimf.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gdoppornv.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gzkmmsbbb.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gdwwcmvee.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckbaghan.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbmuxznp.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbodmglyb.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/grklckmrd.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgcjeilb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzukgkpc.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/geiidstos.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjwoxxdzj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhudjhmy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gesxcxwjb.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkznkcbe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjzrttfc.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grixkpntt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyvokocj.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlgwyknh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxtjbbeqp.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzvoxruq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/grnttlxze.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gapqzqwpc.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgtypkfw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvycdsgg.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmjsteki.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gocjrjzvz.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmipbcjj.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gebkcaxfl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbwlbktle.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gxqlctraf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxjnmcec.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gccesnfia.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goelxhhrq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrjqklnw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gttavmpui.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmdmcgop.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvqvseuij.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkjobikx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdflbyjt.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greacuxvr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gltfipeni.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcntiathe.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzfcsgod.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiwmghhn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaufudbv.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwuxkwqj.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbrvbifyn.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuyagqry.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gencbazvg.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqxzkojeg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gklcnnzlc.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gofozefdo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlwxmsze.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gqqcvgbky.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqmaijkgk.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gflycitiw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/glwmufuet.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gagkdjaai.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gqpwcabek.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzwkqopn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikvlbhhc.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpihugaum.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbozcwehv.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/grhzqhltf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gggfbwbnw.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gntfixgte.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbfjzsyya.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbzlybog.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrtmbstn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffhnjhtr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgkpkomy.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcprdihh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gymlkackm.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/grunxapuo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gwyprfhtu.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gpieinvak.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtfpcbpg.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowdpwurk.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/glnqdtbcv.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/ghmvxblrf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gprbpvobx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/goxxkwlqz.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzushiqsi.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/grcphpuse.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gahcqbytp.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjxszjit.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfqinauh.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gtklwomwd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpklnqhg.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzvmilvaw.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ggjaumhvg.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/giqdrqhmp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudzddppj.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gquivvxch.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqzuyiqi.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmbtalid.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gtybycqsn.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gahaoresc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlgrinac.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/ginhprzlp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhfhihig.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/govzngdhd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gilsbjlmg.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gyggrhujw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyjitgtn.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gskdrawjq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqgmkyvj.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/ghzrxushz.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqtfyyiqu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gyflaintt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gqansmvxu.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzxvkasv.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtqykxme.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gsgcitivx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoiwitnb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemdvjvnf.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyznyznw.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfsrudlu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzewuveh.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guatvmagz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrqggmgy.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gihktvzjj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxteszkz.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gqguodqxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gropgzxfm.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlzzfluw.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyfaempr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbirlyhxc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gwzrdeosh.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gbtwozrzm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgkjpseg.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvlsoskkk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlbdnsjf.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gaczfxilj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxaqekic.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/glnhlqzco.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjunucums.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuywpjqe.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvmipiyk.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxpvztig.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxixhyan.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gdingcxxg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gauhmabxe.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gmvudhggw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gpcyvjwgx.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gdrxnllrl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzznawjkb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gennnyici.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjptztowd.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gadousafx.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gqjraqzrw.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gufwmofup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyhxwhga.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbdsohcbc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/glfnoqihx.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gavjkxfse.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gsodieldu.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/goteymqkw.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoggnppe.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gofpvcrkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbarmvjho.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gwzofbouo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvpbuzxu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqxfeovp.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gaugjupui.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqtgadys.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwpunbavz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtcqyrzhu.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyebvmmar.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gfsrbddyr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvewuwrg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/govhxguwr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwziaqvoc.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogqitnnl.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsnlvxev.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcbmlwbs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoyqawks.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmloomvph.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjhfgpkyf.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gotypxcgg.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gadgnrkxh.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpmsmngzz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryjzvnat.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gctosimav.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmxkubkr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkjssmtu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/ggrpkjetg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidxbjprp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbedrtmcu.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkpagjpmm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghivfaxtr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gkibiqvjf.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmmdpbskr.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuymkqdf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqttkgyz.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcisszro.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeahfypy.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gxvdkhncb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gsxvywhcw.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gexkypmgu.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdrpnrfd.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/guqqclkhb.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrlyfxtv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ginslmihf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbijgdvzq.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggleggorg.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvearinec.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbztoxsum.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxbmlnje.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gbutjsouf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gsynhhjwi.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gkwqgigmf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkggjsvlx.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gexmrtiip.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxsofqea.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfdkbykc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrxvplcw.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gsetpkxut.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/ghwtwchym.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmmdwyfiy.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldevifn.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyabnwfs.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnhljpfm.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqrnoavx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfmvftau.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmusojs.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gsjtnxnac.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbmntewyv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/ghqcirfte.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gipttepyw.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gbogsxmfm.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/grrxqeqvg.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaeskgie.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvufqczfw.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gwycifqbk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsrriafw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykacasun.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/grqbagyrr.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfzqluix.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/goxxocxzt.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gqoprajrm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgnuhqjh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gswxipckd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxxtecfx.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuhwnioh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/goeeqwxzm.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gvqjbnncg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpbvqhkb.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gtehsxibv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gtyjaarmn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfkgmrou.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpmflmbp.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gvewzwktv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvueakyul.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gancwnljt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gksrradkc.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goohfupto.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnglpycxf.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdwkqusz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdatzcuuz.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gactnyrxr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gemfgaayc.sHtML


<!-- 参考信息 -->