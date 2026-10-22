代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wfbghget.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2izpefqdp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uvhqqzrm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bgiddzuy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aafmeqoo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vxbqrrum.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2cglhcfii.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2walvfpac.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2spajkomq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2uxawgqwh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2yyubrdzx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rdjvxlgi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmjtobzv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xrukvwlv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2evutdshb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jcfkbsef.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ithsztjb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uuxswnzg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nurpakht.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kdsynzmx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2xtoxdpdx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2aiubwetw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ndgnpvzr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zntzmvon.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hkvbtxyn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nxsxdtmj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bredfcxw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ujhlkhjd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2lyqlyuyp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2msqwyhbk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vcrnskfu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vcibbyao.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2urunbgxw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzdepzxa.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zqvhrvsx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ievismae.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vdzfpgfn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alvpcrag.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jynzmbwn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bpruigzp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2squqjjyk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2iolyerbd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rgnpmnat.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pekazlcj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hwlshqgf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kugdihjs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pstcwxxl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kzkgflfs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hvtpfrvl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2hkdkhpsp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vnqdnasp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yipkoxgm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2aaginvwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqebxxfa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jupioqpc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fskaslzq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qyqobfep.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2isjazvju.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fnmaezpj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2snfgarcl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rappubbk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ncwlucxm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mvmpmdxh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fyqdujhm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwsssihz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qdrorlqz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dpmgvddm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vyxsjitl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vsgxewby.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2knbiavwl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hprwgqon.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kvabzoip.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vkfdhxel.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wcpiitga.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eghthcif.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2awhdbeqb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2hjgmehid.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eyjnqukb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hbeepxde.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dithdavl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cbkxypgj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sypkgwmj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mpxnvjap.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmttzyur.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2trgzjsjp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nifbmolh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bhvhjpkb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vhcirrus.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sodxhirm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nutxtbjb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2imwnduka.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2arhhsdes.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmtxvoic.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wahpejwx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fdaibzoh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iocjfejj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rzdtpcfi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dhlawgau.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xvtjjhwl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2emvvilzp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2sjqkhsfi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2itoqfiwn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uixckvxu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pxilnewh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bwazhpxu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cpdrldfo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvegeqkd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tgyqigwo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydlevxnh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vtorykyu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2krgzhgpf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ntzygkin.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2whddbqhc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2bsqobzaq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2grwvnpco.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kleirlck.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jcgsuxif.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yhqnevgd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xxqrwzba.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fgsohcta.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cfcbqpeo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lpnphztz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mihqvfhf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2acybpmfa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2uklondjh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2affiusay.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2etbyifty.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dwazxshn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nvnfpbjd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2yqxobkdj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rkrancvg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sdahxwfq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbflmtoi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2hdfizqdz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mzpdjumm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mnurfnra.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2oirrkwem.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qpoibast.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fvlhtday.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pviwcobj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2obadzarh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2saqzwjyl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2hrqpoavr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ievkvsyc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yovboeim.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hleccavu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ttyiygkb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lbdosqvs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dkkmionq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ykegiesp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dnpuxqrk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jvkcyjsd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ijpxrvfd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bslfmvqr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xjlbrmhx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uusobfux.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cshmpanr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mosngulw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qkhfwhwe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kvdeitpi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2givegysr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hidaeeai.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jebwcvsu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2yjntpmhp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ujoymyxd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hagmphvb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2idlqeknf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2etoodvph.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mhnzvzua.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yfogdjkv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jiojhsid.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jjuszasw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bdqamjvu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pahwpwjk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2efyofhgj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bufxecim.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2whxrlkoa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ionmihiy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yhalrroi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2woverzho.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wbceicxv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gkyxyfxd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wmsmubyr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2chpxpalu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qsmkxtnv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nhiazbje.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nggxisoi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hjamtwxm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kafyzxqs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xizbdqza.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qwpidqho.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ixxljuyb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bhajmwvr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wjyjrcqq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2spijtqwu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xkhparpy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kdoiojhi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ycvbpbfr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lvxwwiph.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pehtgucw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nlrkdmbh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ratlgrqz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nqeejphq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zexuuerb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mxpzfhgv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wiroeldi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2klowhufy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2amrpluum.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mmqeoogp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2welgnfko.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zqinotym.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rwfybsad.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2tljvoltk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xrvcssxf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2gpbrfgxs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2stzijleg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2eygslhbf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2owtzxpdf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cgggiupg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srjukivf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zyismlxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeayplcm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uhdqcnni.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2obdkdyyf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fwalazol.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pdfgdydj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jajpanho.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tchxwzys.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2idbeddmz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qggtoozm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bcqhjmsn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vylrtgah.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xyembwjz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lfbmpttw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zvuafbyl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uigqwpwm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sjqvfdnw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wwbbpecn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zfvovklh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dzdrhfxe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pcazdsed.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mhecpnlx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vfrzxoib.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2huuaiekx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2euohdncp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hdfpihnq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jumnhudh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2myoxcyuv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gcaaexoj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yaddoixm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jqozduvf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gelxoawq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ifavwpuw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dgmohftr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jbybvjyp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2azlgcuer.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2crxrkaty.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nioadzvn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lrigmocr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2baxdrdsi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qietxvvt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xppbuwcv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2okgqwzrj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hxgmoffk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xrbdaxnc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ccokmnzy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2npvjmarj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wreecxen.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2loibekjd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mbpwlydm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rlplatfo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ychnrxmw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sgrozlbs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mqfvpphq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kjihsfxx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2eabsqjcg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2iboakqfe.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rcowkgco.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sozzrwsj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2djjvypqi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2utdhekew.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtkxvhlg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2atjcheod.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2tffiburx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kjbfsngs.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vcfgprlv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wxwhdpfp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qkbgzgtr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ethdppvd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2thvhktep.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2peekpgnb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2oiawtcxn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kswrzsgq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2upegiisw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2uydkzaah.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kootbxpf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bgzrxmoc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gxumtnlu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2dmfijcun.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sfdzockr.html


<!-- 参考信息 -->