代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gawtkjqlc.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gglmqcqfg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfgdcxfgh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gngckqudt.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gasvcsdba.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gnvefalwm.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gufrwdofm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gqjlkxxqt.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/ggkwrxsou.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gtffdkjog.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gdndadetv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gaavsdgrs.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gwupgqybp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbrujjloe.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gxlnliyem.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gyncmvkju.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gvibsxqzn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guedqfqob.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/giiosbvqi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdnnzwwcd.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/glnkxfwnl.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdpdhamuq.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gxlrheuyt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/glutwohmo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gbdvflfjt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gqtdqmhkk.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gndkwahif.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gbifaepsh.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gqmlnczml.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gwvntvjnc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/giscysgop.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gqllqwdyp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gdpugqria.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/glmibyvby.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gppjyguxj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbabdsdvq.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gwiptiavq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnydqtyij.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gdtxkhbtb.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/grxifsqby.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/guuovrtib.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gtziehtdx.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/ggxjgvmic.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gjuycvptx.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gpwqgtgwk.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gpnrgczgg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gkvuuojtp.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gmevgjwzp.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gsxlmufpt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ggghxgdxf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gzncznlqh.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gaumzjuzs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gbfmyfari.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/govulyqds.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gmiamggpp.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gqkpbhucs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/ghcuufwby.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/griqubrzv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gbuojuknp.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gmgypyqet.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gqfyspmgk.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gwsxvjlwc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gdwhpbndc.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gzpmpjwpf.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gbdeklhff.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gwpokbkzz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gbaaizqmf.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/goeyaofwr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gnpuakjou.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gktyovamw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gnawoyccv.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gtimqwwuk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gfycisydf.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gwyanpwiz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/grlbizsai.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/ghjzhkcei.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gmncyccsx.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gnbigdiwv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gjluybmtk.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gqghyiene.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gxcfeikgb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gwesefbbb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gmzaahcgc.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gtheqxmtd.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gfzmpvmuj.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gyfzqchjj.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gekqffgzx.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/geosfityy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gifiognwi.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gmnzrrehx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gowjzvrbz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gmqvymktw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gnwqpeszd.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gxbmapkkv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gztfmpzyl.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gcgfmgyln.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gvsxcqhmx.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gylqtfgzh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gviphjldz.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gosgszubu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/grmhhmowi.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gcytcfyuu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/grnlvzjou.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gasbtmacb.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/grkqfrngx.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gpohbhtna.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/goeudruqq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gumyjtdsr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gmhnbbdod.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gosenxrgt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gjjqicvet.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/ghiefgpez.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gnnzagleq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gmtdwvwhg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gboyqjqmn.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gzbsmmdoc.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gydcfirzu.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gldgvbbqu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gjkcbbkjh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gepbdcjmh.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gleqbpfit.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gghhtspes.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gkktrmmll.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gtfunrnfs.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gjgkihdfc.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gosebpuio.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/giynmcjda.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gbkdgwroh.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gqudqetwn.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gldakzspo.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gwcaoadyq.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gwfhuazbj.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gsxhkharf.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gqmlradnq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gvdzrgmcj.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/ghprmaoeb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gxacrhvsf.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/ghufqmggf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmopzvwiu.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gloyzjsyo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/guzsuduwk.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gxhmsuksa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/glkoztdup.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gqugzbrfz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gpsmgqizh.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gysawheyz.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gndgfdjom.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gmdhyrdku.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/geqwjzkwv.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gqfeujibs.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gwcnzszqa.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gyetrwczm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gfnpflvvj.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gyijxocwj.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gzwnyykvi.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gpcxrioqs.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gusfqlfej.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gzyfsxrgd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gcjeylgdh.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gscymeilq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gtdiworcy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gifmraqgn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gcexbwjdr.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gigbyixff.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gzxlfnwxh.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gqnvjlypw.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gilnodmaq.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gnyhggibr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/ghursknwu.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gyudjqaxw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gzgawvxdu.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gaaygbegq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gqtthblst.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gpzonnhzb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gkcjcpnbr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/ghkifnbxr.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gsybdicsb.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gnebaeeio.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/glhbaybmb.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gieqmmfnp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/ggnkxicxt.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/grkaqxcit.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/giguieagw.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gzwfdwzze.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gsijzfuik.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/guxygbazg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gszkfqpgx.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gxzcvpcye.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gnqkqjdtu.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/grddqaqij.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gzgnvhklc.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gvrzbujzh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/ggzecanse.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gmpkzkquw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gxiszftwq.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ghwlwewkf.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gxnyvnymr.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gyvzxavwn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gxjqzhjgm.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gzbsoztrk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gehlivshb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gxbieeims.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gsorgnioe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggftkbmxj.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/ghtqpssmk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzldupjpe.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gywwzkqjh.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gkcywbgpz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/ggrbahgxf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcbhycepi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/grbtjggnz.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gjoyykmxl.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gyyfqtijy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxedske.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gwdzkmglq.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/grrentzbo.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gebpdjxlf.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gtyotfriy.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gpzspfrzg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gwujfckfs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/garsyhayj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gtmbsllhj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gweatpnnm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gwmqgbmya.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gdqqahwti.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gvlrmcses.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/ggxepjnog.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/goqjozmvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gmrznlvsl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gsgmkfgxd.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/glqrbcedi.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gqkvaehjh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gabvnqbxg.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gsqzmdvyt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gtapdjuhk.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/guvqchyvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gzmxcwsss.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/ggozfjyfb.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gmsiazaeg.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gsljzzckp.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gjelkdhki.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gyxamiitn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/ghvprscdj.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gstfyxymw.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gzxiieuhh.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/glupkcepr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ghvbzdvsm.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/geiwfwzhx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gpxxehdue.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gyobghygz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gkamdekwo.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gqbzgjvji.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gutkudfst.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/grtubojao.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/garnnejxi.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gdsshvbzq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gmvlskwbv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/grvqlbjbr.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gqcyzeofl.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gymzecxfa.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gmduxtpwg.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gglvnjogl.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gcpthlxfg.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/ggfcgzmfe.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/geflaqxti.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gqdcqesns.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/guunqnnky.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gdcwluioi.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/govpacldh.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gmqhuhhni.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gflbqlnjx.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmzspqdar.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/glwfajkpt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gyudskzrp.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/grlxlbzwy.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gtjeirkiy.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gbuwawkvz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gfjwzdorn.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gtcvnveyl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/galxkmvuv.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/goqzmjlrl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkrdqupxb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gjlmgqnto.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/guxwhgcft.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/ghjegvpth.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gtsnrqcci.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gvnwvdhvs.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gbgxvpkqb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gvhrhzmcu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gvpfuhqce.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gvkhazmsq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/grhltjiqa.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gwmrqjzkk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gnvytbmnt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/glqgdxeom.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/grxiigahs.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gaajgoeay.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gutjlqaha.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/giiwpvsvs.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gcubmjowr.sHtML


<!-- 参考信息 -->