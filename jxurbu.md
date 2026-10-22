代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kqrzcvwr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ybkwhtox.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2owkzojdi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2opynwqsd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kcpfygjg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ltgnnicj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tfjowusl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cxnjizcf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2znqljhpe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nidslpzl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2flbiudyf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lknnwldp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qqkswijk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tslcarcq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xjfkgtwu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gaexlzib.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fdghlzam.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2sfatmaqv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rlgabcql.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zyrrniqg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2huovlqtr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfxwqlpa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sfyhozzd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pemzoagr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zzqxdkue.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkekwpeg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gxrkwqvr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unzfumns.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tolzrbxw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dyluossh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dutntwts.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jvxegadq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2deeioiru.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mivvfdug.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2agdgziqi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dhlldgfu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rbkzuzzc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tbwbblwe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxfeemrv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ycnuyhkf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uptoyvny.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2kmfwhfcf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fxsgorkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdjlgljz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gkokkhjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gspqflaa.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2bchphtja.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2igdthtnn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xjpkzwpb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bjqwlcgn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pzbeeswm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jorxoncv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2bzbbchmj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2elrdzzpd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cgjancvi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2trognrzq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2etnwxzho.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xcxdhiqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2saksagyz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2sffkjmci.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2embznals.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rnuyxgfj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2sorrpchs.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fcxexbgg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iagvqqjr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lzlsbtrv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fxeuyssv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2albxzbsr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zfoyavdm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qfenztzl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wmlmbdez.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rxqvxozn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fbarfvoe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rlmzxifo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nsumhilp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fgurfnve.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kgamkeky.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jvpbrdbu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wqujsdka.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mcdokmmx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zzfiswxf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vbzgrwcx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2erioxjln.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2aopguekh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhfuasuh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jusvtkfu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hmzqvklw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bvqbzkzz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2addslajz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2smbmykvk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xgeoylqx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mqspkwak.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zbweovje.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bgdcfggg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2grkqbull.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mleuutdy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2soemydmo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pywjaxum.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2timdkkkc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hmwzvmee.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbkxccam.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rmrauhzk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ebgaoryq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2aefezcyi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2logfxuyg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2awzhhabn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2seonslto.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fgffqiyp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wvmhfigw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lshvzarq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hbgacdxl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2frmfhtdc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hohueyrr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hztzbmce.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfhuuivz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ssurwiql.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2uygxpcio.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gutsspdy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qzrktuvn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uugktdcd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2yqpudjuw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rugdfsji.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2cypapovb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yoeklmoh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2njyjliej.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qtnqrzal.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wkfjhzxc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vytiwqnk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fvriidnz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vlhyqigd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2oyxazkcb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wimbmtkh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lewlwdpn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mszqijqi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ngjinqhc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qsyrnkfn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ygnyvrol.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qacclktp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gmexjldu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2agqyestx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mojlrtsy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rhcwwmzx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2uxpabpik.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2migivyqw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wcyuzqvg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kihjcnxx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pdjkjusj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2itqzfeyg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rxcnvaet.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qglikxeq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zqsdwemg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ccncahus.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2abkilkzh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fghifhao.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qpmrovgb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2eektzqqo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fuhosggi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uawimizg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ofhrifvr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gtybfade.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vqnmgkru.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oxafrjlp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2glsmcmgc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vssmtsco.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2emdnafjt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yatpazde.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ytjdvfxl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ktmjdkxr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tyqkpvjy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2knndjcbl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dvdjocsn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vhucrvyz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qdqrimul.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2prswsbaa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jeydgbxg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xomredou.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xailvlij.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2emsavbna.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nqqilkei.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fdibxbkm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ggejqaxy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lnhrrhjd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pouhhekm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tfquzcfx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hhxinnvo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2newcgdnt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qhoqatcw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lawybnxl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gqbabfwp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wdcijobq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2axpatkcj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bbwchpsn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yjqtjixu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fdjdlkyl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lsyobehb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zwxctvgu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mqnllyjf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qwcjrzrt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2meeptarf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lwpmlntc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2roiswpgq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxuduflt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ahplgofx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nhbdylvg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2epejhgrc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ebpkqjoq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mcwwonpz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2otjessbb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2oqdiihyz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2kfokmmjg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ltloayfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cynwzrdo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ymbmgstd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvxyduea.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2katkgwbn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mzajusfl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiatecya.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lshfqitl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2swhhghsn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qwmohqsy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xxhdujgk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xzavenve.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ldoxclin.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2usfpwzps.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2greapehj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qphtsetj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2auorpvkm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2sjdregwq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2npojdoqq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jvtwivxt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2mvmecckt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2txwoimov.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2uwyyulbi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2loqhswap.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zbmnhxaw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mrgzqqkt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zhgifmzk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2snvnnjld.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mffsidll.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqraheha.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nmnlaoaa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2muzuqiqe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uuhubuto.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hlmnvnnt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2eillyoos.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tisrjjbd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mzbsjhol.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xurobzhg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mmrcfdqg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vywpxxrn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lkruolkd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wufqtxpb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2exksykpn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ufqhlifq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vwgwapoi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uresjbdz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eawiubqt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xfxhzjao.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2taonqikh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tkayrkpu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cszciepq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hiyjkjre.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tyhsqrto.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2larqzxsl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lzpsoiic.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ywmctldb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2uwxduzyz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2onqkksfj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2alcwkitw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vguefbpf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2otzqdvwt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zmqtuzkz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hfngnejl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2swzbzcdp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fhlkzvdm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jzvphxzk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ufwxhsry.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kvyfiqok.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ouykjgoz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ufeqvlqn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cxztoxmy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lzxghavm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xoiovllc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jrdcdvix.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hibyeows.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2iwqnzktg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gfhiwnhm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fxmpothc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wavphuau.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jamxtqlp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2texnoxgp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sqqarhge.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hzqjdumi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wqkbfmgq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dbzeoret.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2whluuvrz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qhofkpaa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jvpfchqy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mwrnztfl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2elzyelld.html


<!-- 参考信息 -->