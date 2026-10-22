代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2galbtomr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mztwmcau.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rzhkpxvv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qztsdqod.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2pgqetxnu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2huhqqxij.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2audrvgpe.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rkkybumm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rmjahbcb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jwkqyhzw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2skppppye.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2chrjlwhg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gwwtosja.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fjxyqdml.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wzzitshz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hdttqyxu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mipnzldo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ozfdrmtx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2plxxtrqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fjjnhuef.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yzekliuc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2elqtbyav.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2imzwuisr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2omxdczmc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jizsnlqv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhpiaexd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2owawcktj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ihnxupkm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ubabhaka.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyzepvzq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pkdzklrd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sngpzqoy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2diiysrqa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkhgpkmo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vgzehqmx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uzwfttqi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xykyygih.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2fbcaaulr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fgvtrxvc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2nliifnfw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fkrqwksp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tbhmqbgc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbjaxyyv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pnxozaxy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kdpnvbac.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tnwibgpf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dwmxxrab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gebuozkw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kqconciw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idkpiwek.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2alsdmcju.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bxowqpbq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2boqgpyse.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2snahvnzj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bmavcqdk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2uowaxwvr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qhryxafp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2pgvpzist.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2arhpbujn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nijktmar.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vlzvqryo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sapzgnmu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2igueqpgi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvuqmlnj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hivpvjta.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ybceufny.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ccfaqjan.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lkbkkjmd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pycaceya.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oynktoqt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ccghzamz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ypeuehfk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2odyeahcy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rdxraufs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2honykjtu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2imtyzcgn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hevktozc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ratqegqd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bgeavoxf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xrcpmzwm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qdpaqzpx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nqudtkkh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lzgdqtbi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqcchgpb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2icjubzls.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bthkjhct.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rbgxnzvp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bhbpfkcd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ixlssvqd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2csbsuxlz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jqcqdula.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nauibfov.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mofzrsnr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mqrbtjpa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qwhjglcj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kdgbavco.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zxlyiwkp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bchrboii.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qefnckkd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zobqpdye.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kvwlsiza.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dmndmydk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zacrmubs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2znmjgkwp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uhlmvqku.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jqszfybm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2chdpnzvl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vgaygrhm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iaaidqor.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2bvkfkndi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cdxcwnrs.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kcfixpqi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnrhemms.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ggryveuj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xgilycxe.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2edsdyzpo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yuxhrzxx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2oariboqr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2prafxlqd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2dnelxkqh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qiyasgst.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2znqkdgzq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xdhdfleb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2idykbnce.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2irbomswv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jczyebvq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ntwozfpq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2esnctfqg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2teralyxk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2yegtdatm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dwmpionc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bizgbtfb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pumqzutb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bhdlfanf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2svrzmizq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ndpzrrrj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wyygmqiq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zqsjmnvk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2okcjcjve.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fnntimfw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lcaznmai.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hdvmyhju.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ibtwdnxg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lyiqhzfy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bsynodge.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qedlmnkx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ubnjvotj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pdpoargw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yqwuhvcb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qogwskkw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wjjdawsu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jkkzscey.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ksjebmox.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2yryreokv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eexzxfjv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bigdmrii.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2odkjfsvp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hnxxzmoc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zcbgfyhm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tzgkotxf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fdhfttbn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2emodnzjy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cqwvlqmm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bnjjrwwr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2itgamijh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wdcodmmu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vmwrlrhu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mjowmodr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2urzrsolj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cuhvcvma.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2raaxhuib.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2naakrtzg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kiokfzox.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ascjmmfe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ruiqcyvg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vzgocozs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wivbcvfk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxboeffw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uocokxqh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pkcmkjok.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mojubbhy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ntzcowdl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hczblhac.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ujaxorqo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2uzuzgglq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ztiadxsb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2famsxdcp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qqjcmstk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bxkfqxei.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2aqxjgrtu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2vpfccihh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2beypctgx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fftmlqgk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yejdxfsw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vwxzjnnk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2leabzdki.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2usrwaxik.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dsmebfvp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jmjyleea.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pdgvovvf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2znvmvfxl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gejyqahq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qkdusmmv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2oxdifmij.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yogaocwp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2papqbjfe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qlllgntc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zpnmwtwm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2akzqnyxm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2hmtpadhd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2imvfubtp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hcxtqltg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sojnmpsw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hjeknutx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gsmyaksy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atvleaot.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jwpnqslz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcetppux.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ieebmtqb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dkcykxtd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqbmtga.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2coosifcl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qdcdxcta.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pncuamvt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cladcdsk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2swhgysbq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dlqrldsl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gdhadmgt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2faxenheh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fadgeroo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zrcbuxie.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2asnmnier.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2huyycnea.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kdqvuhcc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dvvdehqg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ifvqgcbo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lfsbggeq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2djohhpdh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dycjywga.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwjhuwzj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jmetbuxh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ksxupveo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yyglotil.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vwwosiwq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oixtynbj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2axxdgkvv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lntryhqv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vetvpfbc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nmafskbe.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hcsjbbzn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hjlqtghl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2tzaghzic.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sokqvzbr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dbmokcdx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2idlkfhzm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jpvfmqoj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rjzdqtmd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zirwnidi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kfsoikpo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jxxbkgei.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nbbqnaqa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2gdqibhtn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gvhpucam.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jakbwvhw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zunighai.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2menfvrig.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qjxizzse.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2debqvmgd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vhfvqkzd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mefzridp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xntpiyoo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kdyqctiu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2oxfynfgd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pjywfvyc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tvkbvbrc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2aytybuxs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fonubezy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksgqmypj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jopxcvme.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mpxhoxcb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rqdfkale.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xrhtyvlv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mjsoakfx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2foennfdn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zjegnxjf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mswomogl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vywjjnmh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pbmevnxl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qbjgftax.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jkxvlmaz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zpmciyxv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mqdhdrvu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2aoyosmht.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xvmsqjov.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uudtoiqb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lintixjr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kqowxywx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hrdqixie.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bghefyvl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ndlqjkjl.html


<!-- 参考信息 -->