代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2myqguvnz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rdfkvble.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fwuqihwj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vrnupmup.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltsnfeua.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2adjpadvo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2uddyswfo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2awfststn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tsvufdik.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qiieawsa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jsqpymco.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2eaohtalk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wgnhcgps.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iysgstnc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2knjxnjlr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gkfdttxu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ibedhzzh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2xjmcwetb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2arncpbfg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2znvniasx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2nzhnspwo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nadzsgka.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nqrqdbym.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vruardgq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2lmsgidmh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qvlikklo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eoztosed.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajtodxue.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vegmmnfg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usryhtbo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ijeydxqe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wcuqlfps.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2autbnsil.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ictzbyae.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jexnjgku.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xdfukjsq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2aumdqoau.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2oznnxwgm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wwtwsfxc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tqscwped.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2levvcvrh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2uqiudhpe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vobflxmm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jdmidjiu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2hlnnvycj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qiimuslh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ruluqswn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2psuxatcc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gircfmvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyxmsqyu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2nfljdfor.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lhjtyfde.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dtuahdwy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mvrvmsfp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ybkuvdmw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2bxwqvvle.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ylcpqzkn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ooijsped.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xahoblnz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2frdbmbhc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2izuwulzj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vbiqsdsl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lticsgpc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ndszbcyn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hdvnhmei.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2garcfbay.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ftyjcebs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dauixrny.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2skthuygi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mvlnrkye.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rzsvgufy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yczexhwe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pvregobm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bncfrgto.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bsyoadkp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rluzossq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rhssquoe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nheqigwr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2pwgybcri.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2whtkuilg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uiaznehl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2eadzmhje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wtqcgzdd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2anunptok.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lbxudggt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rkptqkcv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtaxqsuo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mhdqqgcd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rursahle.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pehscxbq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fcndtvhf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hniaaxss.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2sodornjo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jrtjmmwh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ecdjiknt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rlkuedfl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2duoqqcrv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fpxvbkgv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bdrwulhs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2purtwtdx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mbughjov.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2efndqtou.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ekkqpzyv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mcjfqrbs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdblhgar.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hnwnrrwl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cbxoxfvs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2besdzsfz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rpxbearj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vyciexcz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dwbhambq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vhdcxllo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dviovizb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2gvncfnrw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2odvipyws.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ukxcnjcc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmwdaiep.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kawknqgi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rllpjgei.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2iyexhile.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2trefnjvg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2oszwzwpk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hyocsbxb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lufdhsmn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pwqnplev.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qelikury.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tinbtdtz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fkxvpswk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhriztt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zkqfpwzz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wvyqhikb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wbwvpgce.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mjllhavl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ipdbfbfx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hgwcuzhv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pojpabvi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yzllgtxl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ncroaqll.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ubkpahfl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fxvcdlzj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rgrkctwg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wwktfdfz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jblzzfea.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ccbtbayq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2uyglbqii.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kxkeqcex.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2skdkxzzk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xtegnpww.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oisqrkoy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rcmjxrsq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2laoxhwjh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jihtuuxw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kumoswxz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2svfewcdl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ckzgtmpq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rhrsakvo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mhyhkrrr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2nfvfihkm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dkcycbvf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lqvxdriz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2pvbmstxe.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2thfwhspa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2srdmydvr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ojobosdz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kiyaosqi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sknsbyni.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rudqrhka.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vtfnezbx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wmcvctuq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjzlcnrt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wauvxsqr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yxrutvdk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2aqkosnky.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bdnrdjfs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jaageyvd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iorhfama.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2iqnhtnbc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jrdmhqxh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hucaynhn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bsenkgga.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fmdjbrbi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2apikgfgy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vocgpngx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2oofkdtqv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wujhejdw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2swmwzdlo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2afwkmbrs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qjibcluz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lmkaudec.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gznbdclt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bfmeazqa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vcstckkb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2lahsqsmz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bobrsjwx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vsfadhfw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ljbjjbcc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xyghnqfl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kbhajkin.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjxatdak.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2baafrpmd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2jvwsqsjs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xvqqvnac.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yseewsjx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2blejuwac.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lnruvorx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2eksycxoh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wmqfkmqc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2soqdpwvk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2utowzzmn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kmpprvec.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cmrmhrgu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jpqotxww.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2iseeorjj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2konbgjts.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2iifrchze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwlsmhsh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vlypcyqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xodedqww.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cdpuoxgz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kspzlvqo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ndnpfwia.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jgjypjqa.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ttmhvwuy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2avdofajo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2oljpktzj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zmsszpjh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gxgdghcu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xnpfyznv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bazafxkt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jximjnmi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xaaukoka.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lpcteusi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ywbuhiaf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2stxexdqo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xyphifxw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gafmnunf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ksrnzxth.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bpcypzog.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2porilpfy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2revjvdxq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2geokfzzu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uckazjre.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dfmkvllg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhivlmlp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2igylhczn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ihhoeclf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hothkusa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kzpioaja.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2etapcqto.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2otusuoal.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mghojlok.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rldvyxjd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pdlstwnp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bgrdikob.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zztlvemg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kerhvsjz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2axggusdl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2slgdippr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zltifiaq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2cnlljldm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ishrpgrn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uuwvdnfc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2epspiwne.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qzstxqnd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qykcjlhy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hbamycfn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jlntkprs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pwfzxikf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kneqsdju.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qexcixcc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dxibvcba.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2klfjanwg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pllmonks.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ifuilatf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ssvkgzqq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fmzgqera.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2htryswin.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2raerrnlj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qubqkrwv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pbwmqkdi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2snrtappu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aiuwzzek.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2kcyrfhjw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2prkxbmfu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2axatcmuf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jrhhxgod.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbxqiies.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vlgvpgzg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2iskefjtk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2sefijnlw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2milzgjof.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovmykxbf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2botywyhn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ltnpgcbb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2sspcipxb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ywwlklog.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lfpitium.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jiatlyrw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2menvtxdy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ubobknvv.html


<!-- 参考信息 -->