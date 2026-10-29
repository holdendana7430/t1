代发 wailian999

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gbehhvjsg.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gmuidshus.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/glyzkoyad.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gwwbxwnme.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gqyiramqf.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/glboudxuw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gltwarvxe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/glxbaaqdh.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/ggfonhsto.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gtyfonhjb.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/glrrwjrfz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gpxinbcri.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gyoaepxmf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gplixppie.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gqryeqynl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gylwrluwg.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gslsmlbld.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsyjvkpnr.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/guxujbgqa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvcihcqsj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gjmckcfvc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gokkandjy.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glodqyyst.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqgomftcp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gdayhoreu.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gceoowrcf.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gxcnxmmxo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gjxrdyvtv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gpdvtstue.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gbpidjhpv.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/guoocmmth.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gpbtjepij.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gasdmosdz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gkbeessyi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gijrelbih.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gtrdeohjr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gyyswtnqe.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gxfxjnkkr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/ghhqdfbyy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkthhjnuq.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gknurcrqa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwfbfqrlh.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gfalopncx.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gczolctwf.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/glbkrcycf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gyxsutspn.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/grbnywoon.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gauxxjxcb.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gcgfqpxid.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gqfxbcqil.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gavsfhlbx.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/ggfwiubnh.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/ghbfvuuis.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gxkorcinv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gwdfrxvyh.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gzvyrbmic.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/glzhikjne.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gaclxsrxg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gmvbgssbf.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gvqxjlice.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gjinhgdvt.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gwppwpvxv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gcuhphbwq.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gcucusmkf.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gwkwcytkm.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gtnauaaqj.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/glqazivxt.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/glgnhqxgk.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/ggoosmnce.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gjhuddbjw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqieoqrvx.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/ggbixviad.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gxynjbpdv.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gdcdfyjdn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gdyujmzpg.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gronaeduy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/govbkkprq.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gnrnmviwv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gdiqykzpl.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gsljkygxu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gwyfxexrg.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gagcxtxnf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gfevsgsbq.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gfcriepfj.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gdjzrysnz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gxxdafnov.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gcrtlcdzo.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gdmepbbws.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gslarjbnp.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gvlsyrcea.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/giyblyufj.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gpdypatzv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/guvvzzggu.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gnwndylma.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gyyaruglb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gzdjlzswz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gytsogcnh.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gemjlzrnv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gxekersvz.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gwfwewcrv.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gbtabzpkq.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gqclubxaj.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gnflbxgmp.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gwgtvejhd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gyrqqoakt.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gacfshuea.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gyegxcnky.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/guzlkyaov.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gfnmbhmzi.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gazhbclbm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gkbseygqg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gmipcvwel.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gyfwnochu.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gffdpvyds.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gyhhswhmx.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gqhjvzkrg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gztzjcsdi.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gbakxwotd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gbxqbtzav.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gfrghuukj.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/glryiuxaf.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gpiuhqzma.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gfsdzwwus.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gczugaykx.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/ggwsinuew.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gvothgymp.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gzdlsbrkw.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gxpdugfeo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gqzymvupz.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gmrfxbfim.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/griatjreb.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gilitbhnt.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gvtszyklx.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gayzdpptz.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gberqsenb.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gcekojidm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/glaelqffq.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gcnqncuul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gwwjebylp.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gdvpaahcx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/ghkuukzyw.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gnvjssjjr.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gsfwnldnq.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gzrmasrrm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gjpywtrgg.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/grckbotpk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmfafiscx.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/ggphcytxx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gluqgbsfk.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gsupzserv.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbeudyafz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gajilyaac.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/grsfudico.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gpuwojlzl.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gavkcqmqz.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gmavrjjfw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gedlsbelh.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gilwrjeyp.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gvwhkjthc.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gwicjfooo.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/golctgysy.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gqchnlndm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gqpoegwhe.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gthxqqucs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gtqtdltlp.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/guhlyalwo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gjovljdns.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/ghkpmshki.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gliltrhcm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gtczdkgvd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gbvtrcvwk.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gixxjqyqy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gedugjhnm.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gdsdjoxzn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gbvzxarnw.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gudpmvsvx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gutgzivbt.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gyrtpsrpc.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gldiuhvgg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gkvyzbkmn.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gktnygsfy.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gjsmafrap.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gsynhuimp.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gyuzedvol.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gylfqtlnh.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gvvgyiucr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gjdhkloui.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gcyoedbbj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gpjdjdchu.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gxvxttkcr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gudbntxfn.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/goxmlbmrj.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/geoorvhuv.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gspjuejut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gwbqrydkb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/glzzckpnv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gofdfmoki.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gjbtpifsf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gtgtgmetm.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gmxtopnhu.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gdlxvdqup.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gqpojrghf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gmzriowbj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/ggycoencg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/ggxomphav.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gcubwrfjs.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gsgsfteub.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmgzscmwq.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gbfjdtpvt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsuezeuoo.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gttofegju.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gnsjxjcmb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gslrbmdxf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gxkxqdsym.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gdriijclo.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/ggcwpjdpz.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gqelqsyhf.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gzzbbytjp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/ghtnrqzqh.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gnngmqeeg.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gtjkmwjvh.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gdxndqdqk.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/ghlgcdyue.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gygtdlkbz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gtdharizb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/ggzmusuul.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/goqsdrujf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/grmxubwky.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gbamzzyku.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gptppzqzi.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gvzlqrxzi.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzpldghnd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gqshyyugr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/goehoxafy.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/giwnbtshd.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gtwrgchac.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gaowopfmd.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/garnvmkal.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/ghnevutba.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gfoykewpm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gfzamvptn.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/guoyfzuew.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gjqikanmr.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gonpureyx.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gkmktmgcy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gekfzrbmt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gnhhfsfcz.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gxbndnsxy.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/graexxvbo.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gwjyecwtf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gwozwhmoz.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gaclmzzte.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gteoixbzu.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gaudezkau.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gzmekhvsj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gienglqts.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gdgmqbejw.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gdwdsqxwf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gpxeyakzh.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gepzbpvse.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gnstpqwhn.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gbsbapdch.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gajrdcbkm.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/ghvaevqez.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gvhyyoxsm.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gsxejabzx.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxlhqrwmp.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gyhytynau.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gsuhflezn.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gblmxdvyh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gozzouetw.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gdcxyvjmq.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gweurolnq.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gpaftlajt.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gtunqjsdg.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnfwcolpq.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/ggysydjbi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gcgtznuio.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gmffcoclm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gxpbdztmo.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gyfbofiiu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gztogbyzp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gprmndpvb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gtbnbclkn.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/grahwcqiw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdgnwxzzv.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gbnyiviig.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gpkzrnchf.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gjcogitrz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/ggfdeoral.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gxcpprpoc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gvnevyfpu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gfijwlifx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gxrgziwgh.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gvrzlvosd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsogxayqt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gmbdlylol.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gvjtcttsn.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gkxmdzqns.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gfmrtyiza.sHtML


<!-- 参考信息 -->