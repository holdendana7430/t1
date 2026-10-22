代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kqjvfjhi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tkcvyuwo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ucudacvi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2dsgfaxqq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ckpynhoo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wbnwjmke.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2oavdjxaz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2isirjovp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vvkoaxyh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjezzycq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cwuoazbk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2srhmchbl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ejjknagu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvboxtaa.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xemmxqai.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2myebimuq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2teerjmfk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpdnqhpr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ohjsmgdz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xkymbmua.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rgcxpibk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2nxnlypne.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2plciguvu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yqtprlsb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rslsdncg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dqljefow.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftujlpky.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lrfdmfoc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nzpbhakf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rrvtdvhx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2acnmmjui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjzbaaoj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tsigwkxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcqyxbax.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wwameqfc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pstnhfja.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ajmlfifp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rhxbfrmb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2yelozxsu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2illydlhq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fttwdyst.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2pvscwkca.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ewnolqzj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bvozjwtu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2frbjmcub.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2otjfyqmv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2erqwswgz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ummepfro.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mnomrzky.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mbqktjxx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2txuvcjtk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qqqzshyy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hkogfqvq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2txrbzsfb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xcnugnxc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mfgodzvr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2azggikee.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ayirskwj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2axgwsfmc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nlkhnjln.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hphafbmp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycjnylqu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2argqiwaf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kglsncqn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bqvbqnzf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2zkfwmboi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vrrgbkkp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qaauvswg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wbijkxhj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bclgwtnl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rllhitlz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ethutbwk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jougfehl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pujztqio.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlktrcwu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jpctvbnt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mbnqzcug.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zjhwnhdj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lvyrksjw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjrclffg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2igcwjxqd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cqyfvmbs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vhxydbwh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jgfvpgff.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tsyybmdp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fhxatocm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2cirkksye.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fqohobst.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kynirobj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2glzzzrct.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2utwnkazs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2uavuwpxx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jcceazaz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2meajjouv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vykrctlw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2imwumjwh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2uzseittz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rafwwahe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sjoniuye.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gixevcsr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xcgrukyj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2etnjgdgp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mfjmybuv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uuxcvnop.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qbshnfkr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2urnmmdhl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kyospemw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2itlbmjml.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ztmbspos.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hsnyeegr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dincvxdm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajjcchch.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qtxcadtm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xpxdwfyz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2foaipawx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gnecnnqq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cluwcliv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2uykbzavc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ntbaursj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nzuluzne.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2olvgplnn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2chhnswlk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2eesmxfey.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ptarshtu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dkwkctgr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nlmgmolu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gxoizyvj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2oadfvoso.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ghnmvvso.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rqpdxqcv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fyywdero.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2shelkvji.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2frzpnncj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lrksiltn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2atoggfga.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fpaimoom.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hscudbdv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wctyvcdv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2velhkric.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jwgcypth.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wmssbwwk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uqxwaleq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tggswzbv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jqokwhit.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wcioramf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dpdzgdpw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vsbfejzw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qcjdteyl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ifdhpabi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2stfrdfkv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2tunbzgtt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ezeyulec.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ediwdeuk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kkupwyde.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2oettfeba.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ebkclkgy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2cynqcccj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bopecwal.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2aqkpwzet.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bqmuwcrt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yxkyjxnz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pypexpjv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uwjniiqg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pdnvirhj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pfulqrmn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gbxjmvlq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fgqfymga.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2erodrcng.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lwnndlmi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qbowjbya.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2laknppil.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2yrdgoleq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2imiahlow.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dcwcqdqu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fvktjxlz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2kdmnutiw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2chwlszds.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2syaqxaof.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kfakzwzf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qixcxxft.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2exdddnkq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2asuskifx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ovufcwcp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bngmbftf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xkascetb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bgsxqksk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdydxonf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfgvkvrp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zmnwilmh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqrpapjv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fkrkesla.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xsbzkmxg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xfmzczau.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zhqrrbgs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bxcxhznj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lldrsseo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jfemqhxy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pwpnaija.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kueodnry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbykxtwp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xvgpwoaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2medfqfgt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2apzlzkmt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hvrpttzs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2udmbqyyn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tduduphx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tburdrdn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qnsdnphl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2euuhtkvv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2foweyabs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2awnecomg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sizwwtcq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xgluffxr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cewtckrl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hghcurkt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kjdrgqxs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wquwnljm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xuvtxvhf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dhoafpzc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dbmikwrm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2drilafby.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xjqrpnbv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zatetzdm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lfabsoaw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ccigwxzh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2okwhsyas.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ufsvdhzs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gimvfifb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gppdbwgu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2woczevdw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2iawkdiwt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2osyridvn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kktcqfme.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2kjgvvykv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cwppmpmz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ncnnojrl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zpukourv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tnscpwzn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2efgreenx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hlqlxmzq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2usvffcms.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bxuenwze.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nenpstfp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bhvrjbfx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2geqtfpmk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xbghvcop.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mmwpovxy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2htseupbj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ljmlqxht.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jwvfobow.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cnembjez.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gkmknzmk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zjkqscyb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vsfdyjnl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2osrwvigx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fmnopzgp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cbkdlege.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lebiuzmi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lrvmbuyi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ajqhvgxc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xibwknfp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2sawldztm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xycpkpic.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2quuuybqy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rohkejlg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2igqjbbmy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dzhuvkmf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzgxhiwc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2aevgkbkg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dpsdphbe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2upxocgib.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2trakwmcy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lokieesw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cblljmpx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cbqotsqo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2demdfrub.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qsvronmr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hvgtjmsh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xjnlzryf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2umyrmmam.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hdhhoivl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cyapurfo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2unwdwqoo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kuvrymuy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2sssywzue.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2igrvywhl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2oajvjdca.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jipecuik.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhetjlhp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ximrmnrj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bfkqtqmj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cywkiqpw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2njrdcwjd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gdtqqwhe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bzevzoqn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gaiefygy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nnwpkkfx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rtlvxjgk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dzdmcmgk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fyrbskyn.html


<!-- 参考信息 -->