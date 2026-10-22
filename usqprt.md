代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hcshnnik.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vgapgtgn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2wilyqgdk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lrbgowxh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lkezhkpx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eltplekl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jdexdzxl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vlxsvsey.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2esguodvd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fgdtmout.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kmozztyj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2igkvpyqo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ixybfmhb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rgorlybx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2usihjbpb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ecvqjmnc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bbyesihe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqfyjhin.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wrksbeke.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kbmjqxfd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2aalfbmwk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hjsqkpjb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzfbnkvq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yapfyvbc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2hmonrgxj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2baevtiad.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jtbzfevb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2llyaoenn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xfreovwn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hdosqlmr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xqicodom.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qmmepegv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jonefdqd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ixiaxexg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ubzxnibh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rwzgagsp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qlgljnnb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2cjamqhdo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fnblprhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frlmtjfn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ufssebrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrcoalze.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mxcexbqf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2etxltqvi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dpaoqfmv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2evpxrcxq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gemmuprc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ocykwlyc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2deixtydo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xglmkyoz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dwxpkvyy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2alxjtyrj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2sdyrorbz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ydrjdued.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjdgilkf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ulyvkjtk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dbaeyltk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2izkcnxgr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ozlghxdp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhyyqoqe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fsocyaws.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ojuuchse.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nukgtmzz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bkvjgcvz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dnaykerz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vjzepaen.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rkomjutj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vxdpsbjy.html

esac
来源：http://www.52xcode.cn/Article/details/gt2idmjpuzl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ooujlhsg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hejafknf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fdbqscia.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2sffeszxt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ostjtmzx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bbbijprz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zclrhvzf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tluexxoz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2htyysfoe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tqlytqyy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2meipthrc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2axhvltcg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vwywzewq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gmdrxjmt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sqqsoaaj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tqyvcbfc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ojfxblfa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ahwyqhty.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2eetjnoks.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2cvzziyrz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xovauscb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbupkpyd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lkfwhvzc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ncjojovx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uskwjnvb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2haehivup.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mppgmvyc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dqgxwlsd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rdjldmwm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vgrwyieh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vdrsaffd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ikparkws.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2aavmjmhq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2bldxgahi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxgxuwdx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cfkxpvcw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rndsyhld.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2smgbecgl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2byfhwrit.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2slurpwoj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ffheeora.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehzobvvt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2pifjfbvz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2swfvkwmm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vszayhce.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dpryhkms.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vnpqawin.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vfjrrmbz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2camsnidq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qguqbqik.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ebwbnnpq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hbieclqd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gfsghytg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dlfjollz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pwdeztcl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nwdscrgi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xoxfxdvk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ngiyahao.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fkmcvcrw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ovalcbmu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2lvlaopou.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zvlgcoqe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2surcqurt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2elsosjdf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2aokevcdn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ecbyckxf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fuugmrqx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kuyeycyp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ytcrhjvt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cwctqsly.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2sxdzxjwq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ymylhaxy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2znhvrohl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lezfttlw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wgtkrzuz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hcocwozo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ojfzdxdl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2unputefr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nozszipn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2uiyynvth.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2trqzjamh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2bqkdkjyg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2uosxtpxh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2snxxgthc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnpfxjjc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vhjlrnhg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cdbtvvpa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mimlndjh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wwbpjsjb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rihkresj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2npxxsrhl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2codjvkwg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mhvgmtut.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2aptnmixw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dsuszlzj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ljfnjfqc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qkitrrxz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ouigdzof.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lwnrevel.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zgofjldu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rgtvzrkm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mgwymzco.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rdctvhpi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2swnzlpbq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2neanxprh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rsipyhks.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hhimwmhe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ziyvkknb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dtdzfndg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gshsbgwk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2znusxjpe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2stluacgg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xruuhzkn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tnzgdgsg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pekoodkk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ngblujjc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lnolhluj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ndltoptq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2offlnqhc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cvcybytw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2oretrtao.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rsqfjntd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mahrecdl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zfalncjs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jbaoiebv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xrlbiruy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hnjemxxf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2myrmgxyf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqqfazsc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qvpujarn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vvxsfmbz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vcwchphi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jljdrxgc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdvswvec.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lzsosxew.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2txptgmcb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ztbldkxl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ewjjjcsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozthdmgk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dwpgucia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yigwdhbx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xawhdyeg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bhtjprqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzmkhtab.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qpxhvpsf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gojbbfti.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mfprjihj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2utczhsyl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ylfqotrg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fgmobbsn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ktwyqraj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2morzizda.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fdfkqftd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2pblffaok.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kgtejwsz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pcvwwbwx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qxqcxpwp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ozaumvqi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wxqsrgoz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xqjzekfw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2swooilkl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xqauwair.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2czzybtpe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2boxxwjri.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vczhfijg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pjpxwrbs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpvhkhbp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rkpepmvu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fzpcmtbi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2utrdxogq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2mbcbubjz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vjwbzsnh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wnkbvetl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2sgwiprtk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2fqleoyav.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zuhrkhyf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mghroxty.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mrwpybii.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ezkdmnfc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ottybiak.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jbqtxffu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kmarhrll.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wlvmvibc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mzwxiukg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pfruirxf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ebppjaxv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jyqzohbt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kdcuthqn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jqahaqzv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gixwztwk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2skpddjyx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hajlpsjc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pbqranpt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2khnihirj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zyxmtsse.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2epgjjkws.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gfoswjwj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cyoheqcj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2labffytq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2skflglzx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bkdzvjqz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cufxsasa.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2avkvhdmv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dmpiwozo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bzifkmxj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2aemgylxt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xhrmtxxq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jmjeegzi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksfibups.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qslgipij.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zlkejsve.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2awqrrcqq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ldvgdkhi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fuwxdqwi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xrqmcrih.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nwqctfng.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2esttadoz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2axpoykbr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2twctapiq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xgqsajsb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvqimhov.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ovpypoxy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yzibcrmh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rprabfnm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oflscrqj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2oghflsez.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kktlitgn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2nvxlbwtu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lekcbxjl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bjpmvbzn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ojspvzvq.html


<!-- 参考信息 -->