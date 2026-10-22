代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2cfanvzgr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fpxgzptb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2afpbqevd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xjirhuxw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lqdeicrt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jkimhiyg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fvppxhdi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hdpnbwkj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tgvravvs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jsaqkxtq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kacxpixm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fbwiyqzb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qjekaqip.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ocnxzjlq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2metlnedj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rmubdmav.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2innijhwe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2azbuaydk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2sptogdol.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fytgxeof.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2suutazit.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2sldboade.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2imaslalk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tlbzulxx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wvfdyhpn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2suhumikk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dxgjjmuh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zrxgpigb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xwhibilz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jflkskbh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lrabrqpk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2arthjkni.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rlrmqjxy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zxqmaesc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2udogrwpn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2njhpfkhu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rrybcfls.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uaystoch.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fczlizrz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2crrkpezc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2yleowsnz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yfteebgf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gkejhbpp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jpmrilpx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qapsnmyh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bvpqvabi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dtlguniq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unnwybvk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kcfnvvbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxahhmvw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qwiozthd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jmssnpee.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fqlpyrfx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hgcckopv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dsluboph.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nhjgglhs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2sqgyerzl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dewccppb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fdccqxle.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xcpjznbt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nitpiixy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2donmycrv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qjmbavfm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2fiqbufbz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sgalwjhq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sciuxmby.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gbisejac.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dsborktg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zdwzlmoc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pnefpbms.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2trkngylf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hnexcttf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ivybzhgu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vzfvmdpn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vlqhavip.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2innpzkyv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2semqermk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2anuhhduv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2pxvarhkz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uwzytior.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iiiagwoo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bbihiuhg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hndfrouu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ikrlpptt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mjgipuvm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qtfrjcbr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dklbjlos.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2irpmpgsk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2achibkil.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cruykqsv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xygfeijh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bjxdzrix.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2dwxhuafq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2bkkxlnye.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2allrjdkn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zoxbzlpx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dncgwgup.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2deqryows.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cobadulc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lskbqbsr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rmsptnrk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2btjxsvuf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2syaegiua.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zcvgcryt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vjhfvrof.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2nkposlin.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xncvolsl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2syeavykf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ifkmmeyu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2dncsnosv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2miuqwzvc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rpoywpab.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ywiqvmbj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2udbqyiir.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2yelkvvfs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ggzdundm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zhftxwml.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2yrsczfzl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tknlmqxo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ivpnabbd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ynjapbpq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2sfhlmerf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ybfuwyaz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fgbtlhhg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2recoaodc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fxdcwwqd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2huqxrctb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uxutdpou.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2btyburek.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2layojnxq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qlecswyq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zwqkojyx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pxsaxkes.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kctguyun.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iqrfelmn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zzwjgfit.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ymwrcsom.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nazagsgf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bsygogfm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmdrnuwx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kaeapiog.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nljsrtoq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2laoffiec.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qswpvlsj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2huxlnwtv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yyzpfrsi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bssqoxko.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2styzomsv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vpneilri.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lvsfcubc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cofpfcgy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2mjbrmvox.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pdphmmzn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ocoqsxaq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kgrqltmp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2izgywbac.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cgwtryru.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zxutvyij.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wwjrurkn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sptgavqu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nvkqvrgu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2byhoeehf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wdambklm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ujptkbov.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xchagvmz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xoiigayc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wtoaekzz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qloyyyhq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kduhzscs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2miwwuedp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hlhbldho.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jkeveuwq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gkxssdyg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qtrmomvv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pdkbrnvf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2rfwvnxap.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zwfckacx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cguijhjh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gytkojdj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2luwfwmtl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fhhtqayu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hgzjllrb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2iffjlyuv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2eifbtgin.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kfbfepas.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dkmhdqsj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qjnhukfq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2oolqryrt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2megtzqie.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cgupynpa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jkqrgssh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jrucgxxh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hpctkxya.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gfzmnjnr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2awzyexkq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2balkizqk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fgfrmvqs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2akqjjocq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vmsyqgdr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wtkoevdu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xvyybawr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ybwbwixv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jxskssxz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kstkwkwx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ixxmmnkb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2eufqwhcd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rhcxzaev.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2daqxfabd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vzcbjvqt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gdmiwlws.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2eciwlmbu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cldfcoif.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dfyorcvf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2taiwwsuo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2acycgpeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrirasnj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xdodrckg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vndguoiz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aexnhqhb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2epddrblh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqgkpbnx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kbjwednn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2azufuzwu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lasqfifs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dfjldgsp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nxluhdis.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cmagipen.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nxttmuzn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlaqpwms.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2adahkhwg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gflzatmq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mtwnepaz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2layhhruz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gxrjiosq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zgludpsj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cydnmxez.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ecruhaoc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2apwykuvk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2yfnswkik.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lymielrj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ylvhnyqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fwknavfu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2acobpxnp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wailapfi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mcknkuev.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2luldrrgj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dcjislua.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tqllpzhn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2oajvrerb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rpmafbap.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wyylpqhf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mszwfkqb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lwiqptvm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iqabdwbr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2swyfxspv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2epcxeyyw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hjuwcnpt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ewsjnxxk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2guzxmmdu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2llldksqu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rznyhnos.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wcgdkbvk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2snppammo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2duxwuzar.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kbctvjdg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ycqnybdf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qlkuagpr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kqjijveb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yfqzqruy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2azgitbwp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2igupcxby.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2glflwveu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rhhwwsvh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fmigxgfq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bkygbpym.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2loczvhkt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lknwyvjz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2syyaizuq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2yujvwdes.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2plqgghki.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wecfpyhd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2idliwxat.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2conyiicr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2puiloaps.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dqpuptni.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flpvrelo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqstupou.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xhypkouu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2byvtdeyg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vilqvtao.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ovwageox.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbtannmh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rvwsbbuw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fnlzkzab.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rzrucrrp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cfpzbver.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mftzcbha.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wfgfzydl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hrfeqtbr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dtyqbwtf.html


<!-- 参考信息 -->