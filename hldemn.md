代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2dlrytffz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dikqtkrf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kxfptjnw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2yyhqciqs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cktsgoex.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xvxmhhix.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nnciwoaq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zrabluic.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2upocorog.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2teamsxnn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wrozmzhx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jbobrifh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2lninxnly.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hmdslkka.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vxcalhag.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kjrxdvlp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xrhiaojm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twlyqmtv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2soswtazx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qjbuczkp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tvsyrnal.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohqzagxh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dhnkqehd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lursmamr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2owlkuhdb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2boptekvh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fxzmfatx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2aonwgopy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hjidyehb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tvstowsj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uwzeomos.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kloiqele.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2uovhwdfh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2kvuwsmol.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tstrbllp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jllvulal.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lcqdgchv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgklsmuv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2aehfrsyd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wcytvqfy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2aczqxngb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2stronkbf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2dpogplmq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wvgjillc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bsdfnlhw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fjpssfiv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2adzaijyk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ekznrxrr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2umhwhpuw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2skramopr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tscjkaxl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxtuhstp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qywjjcgl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uauyzbnf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2umqviopi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dgpncpve.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ehlnoaiv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vcsiwfsh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ecyyqeyu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fdvfnvkh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2hwhagvpx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pixsupoq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2waxrzvxw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jpmedyyv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dwmvpbno.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kuvghkwz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eorhdpij.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qnslpgpl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xercqvvw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kejmhupm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2trasxpvn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2unujyxyj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wrtyaphf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gnycielg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cizsvkkg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2fsqncnta.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2oxvheaxr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2aldgnttf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pndpqsam.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2girozcjj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2imgtvnaj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tjmjxbsn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bjgmuyun.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zqpijtrs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ejlvcevs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kctieziq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xzwhdjpu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2iikdumqr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2romkkkji.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jvzpcvpq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zctcvcxs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lhviltwv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iuxnedia.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2johispdw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2moxaaquo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xskopvfx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dkqseiby.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xcixzixp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ohdgmcti.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wdybtkhc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bkiyorqh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lfktmouq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ryvximaa.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2znnmdtyx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xhxynmer.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2szefpjyo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fpkbnbzr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2gvjrxvrg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2okqqrnro.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2cdvbqzil.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xqanowgd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ijhtuvah.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dfyjcash.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yazqkwgh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nplbkdld.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xhfqvazd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzihmjrb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sihljglz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nljvmffd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dbstazyf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lhsahzeq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nptroida.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2darpqovm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dlhjjthx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bldlurld.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qpmyvkaw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2uxtdwnxw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2adbvreii.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2roiulvww.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rbcbwmjt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zazwhppw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lmcecksr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2podtvvmo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cqrkzkdw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vchnwegv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rdseizrq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dzluzxyn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bsksvedd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bxkuwiom.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2khaindtr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jsgzhhjf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2efscvyqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oivbsjvq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qxmzckwk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nwnbjdsf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qckaxuhb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2asysdmay.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2axoxchnt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cnqzhhqi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xeugriwd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bxgjcswo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cgmlqogc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vblsdtrq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2dudfxzyd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nilqqsmf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dewgxgwh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pfnarziw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kzqwffkj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nlyqrrbv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xgdqmmui.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2oqbbzatt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kyezhmov.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2iulxvanf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nkfzslek.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tjpgkulz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vqcxvycf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xtyzrlth.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ghgrcgdg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vmpbbtww.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ptepkzyo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wfboivfv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2jdyauguc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qymvqayo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2psowhijh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ouwwrzdh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ftlngydc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pgjuqkxn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cpolchgz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nfmxyayx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2baknpamu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yjtevrei.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2utlvhmdp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2arjiubbw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ocxfgkpr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tlklckco.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2gcgjsjbz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwgamsmq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ahvhqavz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zegicshp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wcjszjho.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2svhielyq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tvybddyt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2aispxszu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfxcgxvv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kqssuunv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zdgchkhg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2myjmnihb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2omghembe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2uivvskto.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kkligbnz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pkupuqwq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nunncaxs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2oetuaucf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfycniex.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dsuzkyqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrczexrz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fniqmicz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2oglydrjg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rwbcwgvs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lrjjwhxk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nmzqzoxe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hlwtpocy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vtfeseoe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jbithhka.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vqypkbyz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zyapfdeu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbhvlsu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2akbjaijs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gaykvudg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wiozbvbn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hjkcxxig.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nwgpswow.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2uoaiyhft.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2sevgkqdo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rcjyfxfj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hpjcqmbl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yxfynmkc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2iaaqmoez.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ypclnkzn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mrfvgtzz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wjfcejvs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pjwshpxd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fcdtgwmq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2moghmmyb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xnxrdvsu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qosgttjj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2awamyxds.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ispufmdg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dtcjejhk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pzbigacz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gcxwmcnl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kwstuysn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ppihnexd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zvayemag.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mknkfktp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tkwdnsmv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fxtjhgsf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mbrfkcwj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2oygxnpwa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dnsllytz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2byqaxoyx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2afiiqcph.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rmtyeidj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dinkdsac.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iymdxbvn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2herafdhk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ratmzkdd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cynhnjea.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yhzgoeab.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2tjulhhhk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ciqsicdt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rwednpet.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hurehpnr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2amigpwkl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zxorqlpw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2imzsetlf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zrknlpwi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ydhhjefp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2luverjii.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2whqswjzh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dicwiqqt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yjhnblge.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fnudqqok.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2akunwjzw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmqwwzzu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2insulebh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mbtidgpb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2umdckywi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hovnrplh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fdazmmti.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2oqjsdvrq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ledgtzil.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zgpwdkrv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bmwdwupq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xgdbfcqw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2iejqvpec.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2afjuyaxk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pucpdfsl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wscbsdvq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rwftrepc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vycmbqhx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wogahwfd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ceiiqksi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wtftdunm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvcvfcor.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2puvephsz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ninmuwrq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vhdxfnel.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ljnsjlpu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtsxemew.html


<!-- 参考信息 -->