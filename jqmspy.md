代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qypsqhyx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qytkqmns.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ztvtaegh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lkbpbjog.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gcdstqce.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ugyaemfb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hfoiglwb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2crxktfvv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kpqmbvle.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ryalflwv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uamunbih.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yfpactdu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2plmeuipq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tjayinbx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uqyvygyu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qmfnbsra.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wywyvkgl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zvoshhad.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hizbbzlw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2budrmbtr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lywxbchl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jcwiffra.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mvcmyuvf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krlpxaoj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2lwombxyt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlicujkv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jfwvntzw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hcocwalk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fsfsxknl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2stqancdx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vqutlodn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dzjsjvhr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2abqegllr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2albnsqal.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rniptezr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cpaoaqdi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2orhaicjl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mpvkxkjy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2raaybnqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trmqoekv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tvtklavj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oypzlolt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2sffvfber.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dzltrxvr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rrqrxyxp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rdbiotmx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2uuhtrjxa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qtxewply.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kofewjym.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdffdzfi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2oecjwhxx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ozvsmodr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdjitcea.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2onwuafwu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbsrfofd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xkxqmlek.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yzrxeeit.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2euvuyeqo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xwokjmnb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2egnagqyh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tpsdtvug.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2thnmjhqg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pogcaxea.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2czojapsw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2phzeofpv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2oiexxjwx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rfuypcnk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2djqcigsw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jilkfhva.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fggiozfh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zpeqrcqw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvhmjccb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xuywlvzm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hgaeztjv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tdvhdqcn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uibvblfa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yulyhhrp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jcchrkwe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hmhmdhim.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rsopljwd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lephaadd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rhfxhteu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fqnotoev.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fdmlkmwz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nseqkfxp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ndsecejo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2agvvymeb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmadvcre.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2yckoehxm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rrgmwcyj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uboontlk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2svvqsehg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2uguzrlnw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dgucimcf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bimgumqw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vupvtxzb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hockusev.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ipndivws.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2uylxzhiw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2okdjvuza.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xgcsgaxg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wuxwilin.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2raulfgpn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2alwolpmf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddcewfkb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dvmsuhft.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2azmxxvaz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2oddqgays.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhnywduz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mcemaofh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tczbgawq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ptwugzjg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bmoqgfcd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wsvklsna.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xseaelpz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2oerkejka.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kkvrkbrx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wvddnlwz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ggwzurmq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dkcwhedp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tdohrseb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ixhkcbme.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fkdbwgkm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fcaaofrv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cllmafgf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rrqzljlo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ufensfbv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mfdkagzd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ularzuyk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2meeoylnn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2lqhhbtby.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2isiltjxa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mlsrczsf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2lchuubce.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gapznktt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2itrjhmko.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rqaxlhdb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lxetgabt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2iyjrrmkx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gwtvgeev.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bxxwvplo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ytnecrgz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hkzwzwoy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lkmnpxhy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ctpjskoo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2acmwrgem.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dfeilyeq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fdfxojgx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jdkmklmg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gnpbbryf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tjnwpjly.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2faiiawpw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qjfgwfeb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldorcukw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rdeihxuy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ctvvadxp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2teudwfov.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gzedcrhz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vklpdfbr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dchblytb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tsbashcp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rqrshqqt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fpxgziwz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pjvqevda.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nhcryxan.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xqgdzodk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mycxgpvt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nurlzgzr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2taaljrmz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fzvsbngt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2oruaupkr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ednaqowd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2imfakowj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qgpasbbm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2crzcdrik.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vhzuxzeg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dtqpyzes.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2windybki.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2suifxjcw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gynwlzcr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jffvrcqx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tssvwtct.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pqsltmpq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2svqmbbnh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lfrpjzow.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yjkocona.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zhskvnuf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oivyebzy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dqbfxvzm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uyviozdi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ytgzkyei.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jfszomrv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zwggtxdj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zyanokwb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pddotdxp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bskeifwm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2volymwpf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dkwpcidb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nrgudfor.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tyrfzgtz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wrizhcsy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2czqofvgz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hmsgahuh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qiovrizo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2uumtfdek.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hfxascil.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ghojyuyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkxqurge.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ewfritro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sodjdhbf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ovvicbru.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mtpaincj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2libepcin.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2anuwroju.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cgvtvqet.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rrfawsve.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cugzvykk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xvzwzfly.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rgqfuooy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2smmbqcqa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gjhnqids.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wscektxo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jrjepexk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ofpcijop.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2kbvyxgex.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2fhmzbxho.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2svpladuy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2alpyeijf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pjzpqpfh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2sexxyzvi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dazbnlzj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqdiwzxm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rsmzqajo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rhaqrnvs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2deqfujgp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2tvjmalzg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2saexzrqc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qkxqortk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2viyagtuz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iahqzakl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ikvsvqdz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2aqijsnpj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uzemqpqu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2taskibcc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xmrynnyk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ypvtfxql.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2icmlgcnp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ltepjcaa.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wnofquwk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2anoqrdqt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ylxynbst.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2duuhkkfg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zxqanmrl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wbfqkexb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lbcilydo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fwnwbxam.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cmrvyili.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2oikkbwrb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ijxmsfec.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2doidodva.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nwkzsmsr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rmulayti.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ppgeyotb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zfnogknv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bcoyrmfd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nasjcuaz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vnlmltcn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2nspvvwge.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zxleovvx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgmzjpzo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nklvcxou.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ulxwusds.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jfnslqgb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bhvtmbja.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2krffmxqd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fmbjwfuf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hislpazn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bthpnngc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fkdjsozk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2nqyzqskc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vffdeosk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zhaosvpc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2noduasba.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vxydusbe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2puyikgnm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zqykyueu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ubyneyfp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cknzcvbj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zetxtary.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gwbqgyzu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tilqhlgd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ujbbniwp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2alpaaxiv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rtpobwax.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2itwrzapb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lbinicoq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ticpstig.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2oxgihxci.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cdgyvhse.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2mvelsbld.html


<!-- 参考信息 -->