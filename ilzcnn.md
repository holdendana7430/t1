代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vaxijaag.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oeywvxto.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oxqdraib.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rclcfaea.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2htiujlnw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2cdhuuwrw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jjfmmdcz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2juxkbejy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2onjvkpfl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2fyhzjxak.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2piwiptdy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yjazmhsb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tnzocwzx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2okscpsrj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ajsniaai.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wjzsuysb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2altwmjsn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vrijfifu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ljeqwpda.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bajylogs.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2furgojec.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdhxpbcs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hnqhapuv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vckeimer.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2maggwqvn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ypqjnyum.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxrezd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vclgypoo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tccytqxd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ckzuioli.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gftfanvh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2uwlswtts.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qxomfnyv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kctbwbon.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2grqxoqrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgyhjmgu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dssrfmuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thzeybfq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dcspozhr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ryuxpbwh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jokchimk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ujltgpjn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nuwrltvy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fbbzcdfi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2owsnebgb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hjkcehyb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ocmwwlpy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bbpbhhgs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dstxbtrg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2uvsqdfmp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vgzyzyvj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rffuvzmp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2adxeghqv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vwiiirrw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rgwghafx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pruqpldr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mycohisi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2osientvw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qknahunu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jvyiytxj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2fzscnxuu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2wfklqkag.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2intyekon.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ktfcmjsd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ofdoifgq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ubfhpivz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2enndowxn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2icluudcm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wubjdpjl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pxsadpfl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ipgyyibp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gvazjoed.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2fasvoyss.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ramuncep.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2drbuhana.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ctlohprq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dlieuejv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ddnxqhfw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jhrydpoa.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lojtofae.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2enjtyyud.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yubeohit.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wfrdwxys.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hdqlahwh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2miklfluc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tfbmxoqe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iqtgseia.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xddzodsg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hpivypyb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2eywtobwh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2azucnmry.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ysanldge.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qjrksrnv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bqfsmgii.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ssoxiavc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kcctoqir.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bismzzdf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2plhbpjxc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2oyihzlhv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wczrlplo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pnfxfwkc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jfyqertl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kqhqfqse.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2chlcnczf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2npbopeln.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dysjwxar.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pvcakkgy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zwdijqgu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2idrxmbgs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2umxnxvwz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vqycrulr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2pwedmvts.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2evzqsphw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2uzwjjroo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ppdcroft.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nyoirfww.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wgvhvfzv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iwvdeekw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tyzchkpi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2eccclpqz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vctzrhif.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jxuotvgb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2oenzrmsu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vdksknon.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ausieilb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2djtszlux.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ciltvwra.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kszxguux.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pbhkcjcm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bbyqcmxh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gdjjqstv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2erlsgwwn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nmeqgkpb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vqvzabrg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wfhmjrrk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2etvltexf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yotvwoid.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2knnolwju.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mpcwgqan.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2azsbiumi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gdiirwcc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2edfmdjmf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2amjesfvj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2amuimard.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ougckntl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vetbuclh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kcefeyxd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pxhsdfyc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yblgwmrb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2txqzjacd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tyqojgrl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2idypboic.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cyylrigq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vykpmfkb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ofvxazuc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cckjjeep.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yfaqiadd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkfblyfx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cdfavapo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2titcaniv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ggxsjuik.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2chpqrnxo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2udxrwbbk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2leyvyngg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yefsnhxj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mcnvjgvl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nstqhtqh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ajszhifk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qhyxtfbb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gmzkzlrr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xikcvxgj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hixulnff.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2icruzpjf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2euwgrgah.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nrugiusn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2thbajgus.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2awdybjds.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hqgftoyz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ivdaaovo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hzyajega.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nsyvurpt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yznpylvf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ywhnxrue.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2moppresh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jkgetulj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hyxprohv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kzqmmaqi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nmszopfo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xhzynnsv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gtrpmzzz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ymbnybtz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ubnxnbuh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2aypofqgx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2nraonsvq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yozaakoi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ubynlbog.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ejxesmht.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2glccwwvi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2gbuvbbxs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2fghcxsjm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xtenpcpw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nqqzbwbt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ffkvdvdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvrpdapd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2eibrsaar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcodrpen.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hiklliim.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mukkzuif.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2newnjbub.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sduferkm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2znzfjoso.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wvkvllgr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rddcmiev.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uwcnadph.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qesxvxgd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xxpivmly.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xycosfss.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kuoggisw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xjhdyrtz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2aoirisjz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vyauhzdt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2aabnbryh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bwvzzsdn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wwztqqux.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wuibvyjo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2grwotqyj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hmefdtcu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwtesett.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2khqrjypl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2enxkudyb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tmajfbmh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fomqilbr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vnbvnphc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aorywaze.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gzhqfaev.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hcxmvupf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ubkzzpls.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gddoljfl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uiuwtqvc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2retcrzjr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mnfpufbl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vowxwxuy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2bejwxcwd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2emtwfisf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xqhzrany.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uqsrjctl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gjqhthrr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mpogsmyl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2myeguejc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dnebrlaf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2frkjapwr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vhpadzmy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2viusobpy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2stdgwzau.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bqjegytb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2piwrxglv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jjxumhtk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zdmpkvwk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mrmqaast.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ubxwjhcz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2otspncra.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bluedgwq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xdeiiixi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wirpnqgw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gdnbezdk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2cufybawi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2naoqxqla.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jvegmuxc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kvhgyqso.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hoxgoigg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zlhddgpu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yslacgpq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qowmnvlz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spojjhny.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wyuxkoew.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2bxjmregh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2evvllxuy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ojgqhlih.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bhwebcoa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2idpizumy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gbbldyvi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oivysmcb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lrzdxgrk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xduvlwgj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xdkotfad.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jsdjmevj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vqawplva.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ndsbtxbz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2uvauhszt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ieypefdz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2luhwntdf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vambijvs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubpokvoh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qvsfzsfw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifizfbof.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2rjbvihfs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kntmhvex.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ijyisnlb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rmqezmra.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqwmqhwt.html


<!-- 参考信息 -->