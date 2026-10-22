代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jtuwipqa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ahiuvuvb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dosumyst.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2avavmazo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zhskccml.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zugtkofh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hifhdsxn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rscljhay.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kgumwsfs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dmhtajja.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2twqawjlh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mnormzdr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cdykpjiq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ketlpvcy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bcrheicr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ikehpxjd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ugvpqzbm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfzslhqg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qqjolcre.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehuoxxbs.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jobjapji.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dsrbuetk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uulzdytk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dykrhmim.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wfftbkxn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2juhnwlwz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gyotiddb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ezfuowtt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fdvigiuu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2wimreccj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2kcjjqmde.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2bpcvjfvq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ykbfikyo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yiybvpnz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jesspzyp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2guywdvkr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2huzeomqb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pcefwgwn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vtzbsnwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejkyvoeb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lrsqjynr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxrwqoop.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qwuxvdju.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2moomfdxt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qhikitiy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2juiypsic.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kbcspheu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2olzglmeb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2awixkvrh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mrpbmhrg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2siwckcuy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2agmhjwzh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rgdgivgy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2iasfsvjt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ecksgemj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lcipskxv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xngqwqke.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ylcxeycx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tcfhattp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wkdichum.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hmolvbjh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wejhitub.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nseqcvft.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bjyjnxjs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2asgecfua.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ghokxigw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jbwmkews.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2leousugi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mnyhswov.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2spmfxslq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rifyqlsp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pbulqgia.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xjskebnv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bwkflbay.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2grngkayq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rclktxnv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qobssyde.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2dqwsuwcc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nbopynek.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ebqtxcpb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ewpcdkgp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zivbcrgk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2phcyhscc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mumehiyb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhhyztns.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2avwlysom.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2durcuzaz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ervzerrh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bsqqrqkf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2annivrhg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kxjypomz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zrpjfbfk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2elukjppr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aplwrkka.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kflfjgor.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2growzexq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2acmuyhrd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2riuegmwd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2yparuamm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2knktcntk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mvfeaaew.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yecofpxp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vfliustz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jfrptvwe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ihtsrhya.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fbgccvzn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2pqqzlzrf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dgckyxnc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2szpbzler.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rsgpqqwp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lezeapvf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2uwtxvnfh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rubqhtwo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ovtpwkkw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uwuqemmf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2grofvkmi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xtusoier.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2yhhhtvxl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vgsfuogd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xajqchzl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2osgszvih.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rzgrebtf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lkxpoogz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fcpqqbcu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zmjhyuwq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2grgtrmsv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uwdbdjre.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2equpblrv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aaagnrfn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tufaaldc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rhdmirik.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ucexhdzd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bldhsndd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2oewavvuq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2szcxvyyl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xlqrkkwa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ejvajhwr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wexvheuz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sbnqpmqf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hlghxjww.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2edoalams.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2sxtucyvl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qvnruako.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vvjidylx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2urpweziv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wsguvkcm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xhicbwmk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ykszwpyf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ltjwxgld.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dajyecjm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dvfbgdse.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hcgrtbhx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uyndditw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lipapavq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gkfezgbc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2doihukzm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2opvqkmlc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lwgjqncd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2yfcmectk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gjcaszzo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wmiaspnd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iduzenlm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2obrinnov.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ktrwkuzv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ymdihalp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mfdjjtot.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2msyqbhca.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2smvnehfl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vunjyxkd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2whuwjbrh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vwxzvcyj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xhoctpys.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2iwymlduo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fhirngzq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nmuulbre.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ikpjgevp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rdrdguce.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gfkyownx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jlyueegs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tgtuvvcx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2dlduaiyu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mitfakjj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kndoxxfl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ajcyglri.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jnafmbdf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2czytdxyc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2iohundgt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2btbcjxel.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bkypvtfu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tffomslz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zwxfxlkk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mhhiaghf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2eagytati.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pefrxwnu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wcgrepdm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mcblmhwh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ijurzint.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbotgywu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fysbhfoa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2sattzpgq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2otiegleg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2tqsvxpbd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iwlygyfy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fczfweds.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jlmedfft.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2uulnbrrj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dvtfucwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euzotdvd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pgiicuuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eifqnxdt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rojdnlmg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lzqgudax.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqtuerip.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nmhhpzmc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2dtylfnxp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2denbfiav.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wflgtbfd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jdnhzevl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cdtdfmbo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fidnvzpc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgumshtl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qtdwhimr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qsbhsinh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dxphdwsw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dtgrfefl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jivabkfj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2uogashnb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rapwbsfn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nlopzotb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lkwokufd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2myagezus.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sjocalgp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zjguqosv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cphlygal.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xtucflgr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hirdqjou.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nnttufii.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dsoymkzm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2voszldjs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fditilkh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xvcilapc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lyogzjlw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ljzuntdn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vwhtnagy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vthbejde.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dtssaexe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hqomasxq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2glepilal.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jrpxmheg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yrqfsssz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dnfjrvsf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2recbetcw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hohnlnju.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2caeeoizv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dvdcvhql.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2owthenog.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bradaiku.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ektxvlgh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gbtjsopm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jykrbzve.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2maocuyle.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2owrkcmlc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rjasadng.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wqfqcojb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kcbduzwb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zwfvypuc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uqtfuwdh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mfixjhru.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2excgbhyf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rlblugot.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mtvdxmex.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ligidnct.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kpjjpxvb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eqnstemh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tjznsfrr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dajcdvkq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mifuzcsh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urjkdcne.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kgkcxybc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2aswggmea.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jtihprtn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2grnonmgk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ahkrvyyt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cwujmlbi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fwgrzpdi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jjbwpzwi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dzmctlgo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eiotcbgv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pmgvhjrl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qajguxno.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xweehytk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ywflzwfn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mbmykzcc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ctzofbyp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2otwsjaoz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ydebxpie.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvhodkgf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pfknhduy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qensvulm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dwywgtbh.html


<!-- 参考信息 -->