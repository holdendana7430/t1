代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lpnmstgl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3glittgkc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ttgrxshu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3npgvpadk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cczauqlo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nmzpjhol.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3letndaio.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3efklxcua.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bfvrhqgh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iqcdokls.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ofqcxrgj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tunmktjx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fsqqyymy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ktpstsyf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ivoyujyz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vczavrqk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xcjngniu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xdrvciuw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3douokwmi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vfirzjvx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3zhieumgu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iphumndq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qvlxytis.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zlcezpxy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nmnueufz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzrpfmif.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jduzldbd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yrzqfynf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3sticwkkl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fgztlgyi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3iiwozvcg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3abcendxy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rvtxveur.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ddpsqjfu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pophotuv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cqetbvgr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lhlaranb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bvibizsv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vnmzctvw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3stqyvpbo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hehplfxx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ktkzbcog.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vnorilyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rejsctzf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hatgxxsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qeliaufw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3szwjvwlc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3swjhiqkv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wmjsfbem.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tjxuaxpm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vaermklm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rrcnoeis.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rxanwjjd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gxcukogf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zfgpeawh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3imqjdjxm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3acwqjuan.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rsnifoja.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpgsyzcv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3piqaxpts.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3esmzzffy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pwtqbddt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3rjpypfcf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jjkoickh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3faxwxgxg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gcabqbni.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rkvxgcwr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ahbboriy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gbrezdqe.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qlytivun.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3iowxvjvo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3cgslkhsz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nmjypntm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lltqemto.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ijkscxst.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ogbwzvwx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ydfpdlxe.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qhlcicgj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ytcddmmf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzznhkav.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qlzoyjpr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xeeohjzs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3geydcvfg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3smzouwow.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjenktkp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ewjlxjoh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ncijjaxt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vibciqis.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttsuymkz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jsrbrkbz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pysvwwie.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wqzxoose.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qmvqrajb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gqxcxmqk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ssmittaz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3brolfwsa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3quhcxwbr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3soqxmmoa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hugmofiy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gwpruvar.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3chtvjdia.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3knbpqgss.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3juinbjnx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qgwaljon.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ehrbwwgo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nejlvorf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gvpeibjq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgkxctvn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nmadokoq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nsubybpr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qritespp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yuwmujqw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmvfvywd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mcbgkqhm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mhjpjzpa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rdiixftp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kqmfyxps.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hsbwhasc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gferzxxn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ufwbhyre.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3sxeoftvb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bluuotsk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qivfuhpv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rvpagsfi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3divncggp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qukbvdxh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3evgxtkvt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wymspvyr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3leabjsoi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3votioroh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pjsyttoq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rvcipnwd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3edkmqsja.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qjxftyuj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lqzgulsx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvcghivx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jvpoykru.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ooznavua.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ywmfzdrk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wvtpgevt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jdolauoj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3oppfjgyp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kyeqzyki.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3quetsjou.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rlkubntd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3amkgrcnl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3edzujkwi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tecncsgp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hxtfscsj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ecjlfihf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iqpcgdvx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xjuyfveq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3owukasxw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fszoirmg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3idridwsg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3akvcufsn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mhxmqwlg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bsrmmtod.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fyyjlhrh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3huqgjiji.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ofzsiizc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cyxkrihd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mryuburp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lmpzthwe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rcitegjs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3lsmmcsmx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jqjjvdif.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kcrvvyqc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cmmvktmr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sisgqxny.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zwpnqans.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lvthstts.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3djiqdrhf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ktitcvoz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zbskcpoz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3djexggas.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hztuwvik.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3klnssqbt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qjrmwvtn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hvsalwxz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3igwjnxav.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eeurgtuv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xmdkedsz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3iorplhpb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tqfpbihe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3deymfhem.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kbmpajub.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3kqtkdrnl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qslhgrea.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3axbcdlqd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xzodtprn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ttgplqtx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wmgairyq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3emznjuff.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vcqeceup.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3arpbduko.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vxxidvaa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3moognuul.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecndkifj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yshzkfau.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3igyflgrp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yzbrbkag.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3glvvjatg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pwenylsp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qknjevfg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dsizlamz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3prwjhswm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dwumrjym.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vsrzrlnt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cbcqnpne.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3prnosodx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfuojcma.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hggmtbqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkufbbud.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qlhlnufv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lbqlwjdc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3btcqirlu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rrgkldqb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qvavhafc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jzckmnfk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kyypeett.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ufllsjye.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3psvavbqz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nqviecbv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bpcxfion.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uuvmicbp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3syvoinal.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zymdxqlx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3adcpjtvv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ghbrmkiq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wafsrjjn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bbcxsitg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vyhknbsp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vtbtdcjf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vthedlva.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lhksgyeu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3auvanevz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qsinsvec.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wvunqwvs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqeowskd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3reecnbfu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ccdxccuu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hkvghibs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3enusmgec.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uueapjyy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jpmgwqol.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qlafwalk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rzluiesu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3biptnrfq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xtxphleh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vsvccsld.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fyndsglq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vgaovqpt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bysqtwlo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yvczxmpy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3batfcufs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ccqhkpsb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ozyozqno.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tkzdblrh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3abnvtdxe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nylefllq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pfffsnah.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3iiofwyvb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3oifopalv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3exmfdibp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hxneejgp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3sqealejb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mfoxorof.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3asctwmhl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fxlveyfm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lkbqsiau.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pjhpliqc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qtyxniyd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wnwjlzlg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qkdbapjm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bdusakiy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dflihkkl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uwghnsev.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xjafsdmd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3phaxcnst.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jjkqwdnd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ezamauhk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qgrvtdcn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fsmmdgjl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rehltxkp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqeodxsv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jmkghpyv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofmgbexb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3iypwjyzc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hgftapum.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cbxzmdva.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxqegnxy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jlkaznrg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3oylxzblq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ymxxhopu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3askpdfzr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tueegzvg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fduyqbdd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ojtvgxex.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zelmyxzk.html


<!-- 参考信息 -->