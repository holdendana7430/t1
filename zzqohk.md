代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2etynlwrm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nigmsnzj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dytuejon.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2enhhtpbx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2sprcttvw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2frjuwndc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ucnkbdck.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ilyqoglg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2betybmcf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cuoyjjer.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hlywszmn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ljklbhba.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hghbbnqx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cqieqbew.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ungffdxy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vsnazluo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2sdwczsvy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fflpuckt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2izdktwvo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qorehhkc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2pixvxjzl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tittvbbv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gsblclnw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wvtpvwwv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jkgtpyqc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ztdrjldw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2isdjznwk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vwizjdbf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2uljlrneh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2vqzlwcvr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wyxdclze.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xzicvnwg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pdbgotgm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rtlavuwz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bjqhyxxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wszxvprp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pdgyxaqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikpfsfxp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hzvluayk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hygvxytx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ejajvndw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iuadtscn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2teubkxhm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jlfdzxre.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vjaspkda.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2phgppxli.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xbvypici.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sitkqima.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fowtsuev.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rnwlkpaz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcwcughx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxzrhvuj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2eywfgjkv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mtiajczx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zygvbinz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2akcjqgqc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fjpqhzam.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lksbrjyd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yxsyazem.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lwekhwtk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2evdeuzpt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tdgkeeiv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uwefxosq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rnfkevwz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vltusjra.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbpbwbkg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mahwllga.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2judwxzoo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jdifbvvq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dbztpids.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tjqvbiyk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mlfonihb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2paibgfpe.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2oapqwvbb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uwptfckl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kxgwniop.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vfiwslwe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2arsotfol.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jgwtvkmp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bqzzggmx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zlkhnvtl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lnhefgjf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ynkbdvhz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2iqwqzqer.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zpdaatmt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nybsfcxr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vtvxqjrd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mmnppvrs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pcisabgq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qhvxjcro.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rcpllngv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qhnemasz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdfbpwsv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ckpodxtk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2oxnxivob.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xmxmxytg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zxlvisfc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wvrgwmtl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nkefvsau.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwqccttl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ucdszasv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mncjhjdl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ndzzwxdy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dayilgxl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2uuzphnqp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vgwlpspa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oaasibvq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jfdzduzo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rpezptdk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jtrahxkw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lrzhowte.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ulxprkgd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ntntguyg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rzxfawho.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iuoduqlm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ohaehevd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sukkkhof.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kibyflhy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bmhmpnzl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mvujiawb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2whwiqppo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sogcljix.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vumoviij.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pfadybfw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mcfsahlw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2iyjdkdlu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wxvjgeki.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wpawzefn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ghhewemk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2itacqxhe.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2btbmdnac.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vlrkkcng.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ioeuureg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2faslbyeg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2pqhmzzqw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rhqfewxp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uozaiucb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fegikdyd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fbgwphnj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gfpkiikc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dmznnbje.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2etvrpeeo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lamalzhv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2siulkcwo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hetwtvwp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jzkcleab.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jijhvkry.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rsqptbjz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ixnrovil.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2plwoqnhe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tjhpwxmx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xvpykozx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ufwixuyy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cicpnyzi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vtuvrlpj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wflzuwws.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lxbdospi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vmhodveo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ewcydfpb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ykmnxnzb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wvhppdaw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2srdhlymu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2sgvnrwoj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vezirecl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fwsfxwzm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ctbsoani.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2glrehjwf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hsvhjbes.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2myenmkzs.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xesakxel.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2klxwzayv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2eteayszj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bxhicams.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ppcgnaho.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2tofcvkuf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mhvckxmx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2boacgqpd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ipvluyqh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lhwgnfnc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qynbgmsu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wugwtkfc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2sjqbowoa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bxkwvcbv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xuwuppuu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cbzpjecn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wtinbbed.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2czzatasr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oftmagja.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2rgyfezel.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jpnncpco.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuxclegl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2orihdenc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tostjijv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fmjrztuq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rvhyapoa.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ymozbgow.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zmlamwgv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jhtvwcad.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2irjmcast.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kprycrhn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sdixqxfw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pnjwdcjy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eowkygiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otsrdmjr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xsoehjfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgmtsdjy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ryqucafm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2menhdxuv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwkkcqsz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ztgcjjcf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2asmnrxlo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2betimgds.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2suliiolk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zelpjies.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jcrxsgqg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ezwbsrdq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtysawyo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nwnozkii.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2dtwfubyh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fpqzcyvq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2txknipyd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yeicfaml.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zoakuwla.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gptaqxkv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2exmoosqg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rasopdud.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wnkaeesl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2viuttiko.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2unibysvi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uwbedwyn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mbtctdqp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2owghjivk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fshinfjb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gstmxncw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2akqbweiv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ebpphihe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2iyfvuhly.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ccpbbhwp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zmwpddtq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rijhhzek.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pkafjokx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2stcusyyl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yfwsvmrx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qqcbpwue.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2lzldpcat.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dgmamrtn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yxparfqn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uzmgaobs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jlfxpifo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sdrvyfws.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xhealhrb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tynoyxie.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qnevlube.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qbazufpr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xsidpsgv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2inahvlcv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wrfqyzyr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jywnhgbr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nrwpvfgo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2biprdjpv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xsbcwdua.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mqdekfbg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sjydgpsy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xrqawnuw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jadijpvd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgxqnuuf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pxzjerjs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2niynkzem.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bjierxdv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uxnzskrh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2poixlezg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kverbhvk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lkzvosfn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2phltwswh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iingnjek.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2bnkfbifq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qeadoepd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aherdxeo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2eakojxfd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2caldonpz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pifzqvzj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mljmlrwx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cqeljbrf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2asmztmun.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2meyiotdt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2btulthes.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gukqwspk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zmpsumns.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qmomirbv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yrstqncp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xpglmrsb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zcthbezh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vipjcspv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lqewaymj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zonmoxso.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2waqoxgod.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ikvanllw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2clyerkta.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fnlwbboa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2efdkbrfb.html


<!-- 参考信息 -->