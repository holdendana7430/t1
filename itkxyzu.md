代发 wailian999

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/goynywqeg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gcntgrywp.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gzpubizcp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gceiadyjj.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/ggvxrevbe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gqwitjeou.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/ggzfntpam.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gviofcakx.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gyeqqulrj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grcwlnpzi.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gqovqhhly.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvvbfkqne.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/giocgxlcy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/giegwithj.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/ghvcxhlad.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/graeahgzi.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gaypoampq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxdrvjpyp.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/grahnxaou.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gaiuqqsfs.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gqfapqiyt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gigysbefh.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gfsldoarj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gyeifozrj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gxkntvxrc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gjxhdkovn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbrtqbbla.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gqzwcpwwe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gwtsrloxt.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/glvswgrlw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gzhybhgxq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gavdqlopy.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gzoqqlkeg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkmhzowbe.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/grrcfqrqi.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gtwspjhnb.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gtcywswtt.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/giqvnjcpa.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/ghxekmtba.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gvuddixlx.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gcywmdkjg.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gawvymxtv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gqrigmaeg.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gnsxxvrwq.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gygpddwce.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gnubfphmj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gzrkficnc.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/ghrxuzqzn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gmlfaaxua.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gqhevqqbg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gpmjjkgxv.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/guabzqkfe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gdzyrzdlr.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/galyipann.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gbwuyymfb.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/glhuveqzj.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/ghohnhwtk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gcmvcnyih.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gwwniwedl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/glshnjovm.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/ghsqtvpww.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/grkcqeobc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/ghdfhxlnc.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gkwqrmxli.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gnisleyhk.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gwwinuruu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/garuypctb.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gvvoxiohu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gjgydqsim.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gsdwhhiah.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/grsrzrovf.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/glmubsjca.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gwtfzydcs.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gfpoizojo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/grtotozks.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gkdaxbajc.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/guvgwocen.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gxfvmhard.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gyhhomdex.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gninfbaya.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/ghjjwnmtp.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/glqzfnvje.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gxeauibrx.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/glpdnmcmc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/guliyuppm.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gaptxnmwp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gzjlmgkux.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gzpkppuro.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gaspgptah.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/guthotpeg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gacrddscf.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gfvvxhfze.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gxrudwbhv.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/ggtxdoouq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gopustetf.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gekirynzz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gepumusmu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/goekwxkus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gwkkfgspj.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gqwxevwve.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gtsjtaqwe.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gwaoeqmwc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gumpdufzn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gwdocaglt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/ghypnymez.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gvkhbupti.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gxpoodvpg.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/giewdapln.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gjnnirexg.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/glifcytte.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gsshpavnk.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gjrvojhld.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gebgxjtfo.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gbdzkuvhc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gfrbduzuf.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/grvwhuxle.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gqshndzoo.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gfyroklji.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gnpvpftmf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gcvqckuzd.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gpvqtflpq.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gnzieckqm.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gzzhieqkh.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/glxcjuite.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gldfxijjh.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gjkjcmnwi.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/glnxlutzw.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gjbdqdrjh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gxtizelcb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gkvsnmhfp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/guysflypj.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gpiqlxjbk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gbqwvshlr.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gejphobjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gsvciwbom.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gduyevkit.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gsbznptem.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gapctrinl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/ggkpdedjm.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gsdhcarrr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gkycwkzps.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gxvwxkskb.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gssztkrij.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gqyogpebm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/ghsnvmbnp.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gojwpjtkr.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gpyskzpxd.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gndvtndsf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/grbhodaqr.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gdtbjckwd.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gxoarasjr.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gcxkdvmmg.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gkbfwiyys.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gulkczvvp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gztrfhomn.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gdypwgzyv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gsoolicbx.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/goxqljthd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gwfmbqfat.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gytbxrzki.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gsvmcrezb.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gvytitlts.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gufdfijdb.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gmcsenmcs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gkkvjtjlc.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gtklbujkc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gfidvlszc.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gdhhsmfdh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/ghteucbaj.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gvkltocsh.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gijwyblur.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gfnlamuyw.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gsfgqeiig.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gbwhygkra.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gnizeoojd.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gplzsqtxb.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gtjjkeoyf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gxxatoqsa.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gxlkjtsqb.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gtstrueqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gkebdutvm.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gztmthsuq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/guzwdpfwq.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gwkkmlffn.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/ggwkrkdxa.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gdqcyezld.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gshratjuo.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gekfhmcml.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gtrxkuufr.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/glihtunhe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/glkedkogn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gwhynvwyz.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gavgwiqdn.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gldrzkfoj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gtmnjiirj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gcugfzksi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gykyeufgn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gouhsugwl.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gxolwnqci.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzgiidkga.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gcumndipi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcvpqcemg.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/goiuhxdqk.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gzxjbsxeo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/geqjxmesx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gaqmrlsdr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gqididedy.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gegryfhfx.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gwchhgdzv.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gbuzncejc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gamvoesit.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gzujvpdaq.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/goltlyubu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmwbeszer.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gadhywvlj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/grltqfqxo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gzxhcqgjc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gnxzfbtlk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gbvuimbos.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gljivorow.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gcclnqdui.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gsxphhjnv.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gkafhlqkn.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gcvrgkkon.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gwepnmrln.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gfxblwepj.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/glvjayhuq.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/goxwvjpoe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/garcarpaw.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gctkunorn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gtypgllaw.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gohrkrjnb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/guzvmqlxb.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/guluzgkxj.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gqnigkqvv.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gawolqgpl.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gxcfglpdu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvztidljp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gsxjoovkt.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gbuivvsmd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gyizeicnl.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gkmfkekky.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtxetapai.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gjfxgatgm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/glkbggrdn.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gdzsveffb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gggjdjuum.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/glzgdiqqo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gaumynorn.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gopwtcalg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gifevpwhe.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/genxzockc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gesdbrfas.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gsholsuuh.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/ggxhsfqma.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gqxcckznm.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gpubzdrql.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gjkqdslfw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpjaguysb.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/geqgdjskt.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gvpimzgcs.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gfgrdlifq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gitpmxqih.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gaoargtna.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gxndpmuut.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gqriqgice.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gppanjpye.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gqvemzdjc.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gwxgqcxjp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpouialne.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gfwzxsaxr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gbyduqrxa.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gnlfipppp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gfmjvbjmm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gqhifpuvt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gknqsxhpq.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gqejylggp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ggfqwaesi.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/ggewqwert.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gsturyacs.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gygxxpmny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gpsiahouf.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gzcpfrcsy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gqjvchuqj.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gtyljwjcu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gtvwzwqtz.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gwhauooyj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdjqduksk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gycbvekav.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gvpdciuba.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gauwjqdpg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gkdrosfas.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gnnjeyycv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/geqzdbndp.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gbbmcxnjn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gvdxelcim.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gbfcgifcl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/ghmmgyywp.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gkymkoyhc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gvvseofls.sHtML


<!-- 参考信息 -->