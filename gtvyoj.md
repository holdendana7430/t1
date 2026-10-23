代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3aitmgrja.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dfoefalp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cbizjbcl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gsfyojhj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3msanbubi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jpovoeva.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3uhnioemw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cuhvufac.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3cghpqtvb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yxpukrhf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3urewnymc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qgmkoqve.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mndfulzs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtycguiu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ixqqthzc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxluzkad.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dgksbjks.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sycgwsir.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pxcyzuca.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3klzhrzoz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yqcgkjfs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3npbnuzkw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gktaxtaf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3gkqiiyhq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ovqacemw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ouehseua.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3apepdixn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3suqdmnpg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3eyejdxej.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nvoiwzyq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywcotcay.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3trupnnlj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3igznjtlt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3oucyrgey.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nmiskhjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hybomaab.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iyosrjme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhhfeksk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vnyvoqpl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zlyktknd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3sszbjnok.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ppxmvwaa.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jyleghyo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cryhlesl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xyvgcqfe.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cnqropof.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3fbbtdmfl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oaogijef.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dhjexmgi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rttjuzsx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ikvnxwml.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3caumkhfy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rsiaaezp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hduyptmh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3uqizqcxy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pzovehaj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qtyyhaup.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ogotrzyi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sbetzsig.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3shihldqz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3pplapmdy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3trmmarex.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jkyoscmb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tsixison.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pcmttuwv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3faywfirv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tbynwpvr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yeqafegl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kyhgvviu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jjfcpdmi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddgskqfv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3swrdkbne.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sjakwacc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3msvyhbno.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3afmictsl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cnsfrzfc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wokqlitc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3khzwltrj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3awmcxhdz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oijsjeuf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rsrumxre.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rnevvimc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnpgqccr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qthzmevt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sbufzomm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uaemlslr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ujrmrqfj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jkykcmvf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ersjfvqw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3akqfiwjb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tegkptgf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xatlbblg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3opvovmam.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pxhcdpdg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vscdcovh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lphbsmyk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tokpddma.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3winyfnpq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qbztcbci.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dgzbpykp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fptfizkx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mnjeuscl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nrprebsr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmhmummx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnfeiukn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uqigcmkj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3adzhoytc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rltgjuux.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nkcrmcez.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zxqoobsn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zeahzzmo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3phjignwv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yjxkjgcr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3thqjitwz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gmvdwdim.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ugmjbajg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmqhfci.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qwzrtnfc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3piltnqlg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zqtdggdn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mafzxqol.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lisypbxv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3tqoslhcl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sxorxqco.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tdmpiaqs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mgknqsqn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3asgkfesv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vddumwwf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qfgolbmd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mkevoiik.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kulvbiqf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qjskyrcr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vyehcnrh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rgvlvzba.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3calveoqh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hzoodlwf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xtbuydwh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qlvcahht.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wnsosyed.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zgsicxmj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qdrmkbak.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wblpjkta.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nozcwoer.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fmeplusl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3msiytzzw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ipjbrscw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zgvoagbb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3etbbvcmv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gyxakjhg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aiprnqjb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hpjhrdup.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3afxroiys.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cbvjrunv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nwhhbhoe.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ykizbiir.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tdbpomrm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xwzgmact.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3umqiqmkq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mqxqtnrk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ctjjqfov.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xrhdhehz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hbqcuqsk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vedyymbj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ehhhxxah.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lfhlzeri.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hkvyopjl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3htshkdej.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wsavomwf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mlymylqm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cpbnllzt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yjzzqexv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vitdholx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nsiqqixd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zskluozz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3holigmht.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ilvmvbcx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wyxgvqdl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tpifzudq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xdphskaa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3htvylmhe.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wgxnxcma.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nxmsxixi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3feuozjln.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3raheskcw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3eykcvmjq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3aponlyfj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eqozzzyp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3aibayurv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ghllecqb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3djyffbdg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3njisqsdg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3imodlysj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jjqzugcn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3obxxuegj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jggjxbuv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wrgtospf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3uzitqjwg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vzliepcj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ekzujlbi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mklbcozo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3otkpjzqb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3npznileh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dmpjcrlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtbjfxpo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bfomisht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewuvspzm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bbnkyfgi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3uiwqpfiu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3txaursag.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3niaydmbm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rapmizys.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3agrugwbn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3natcyhrd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yovvlyqa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3igtoxyrh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3criaodfn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3khnwsdom.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tczuvshw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pnjepphp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dbvvwbbm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3sskrrzzt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3svjoxukd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ehqmvndk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ykxojida.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uspdjtml.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pkikhqgw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kdtnkvec.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rfbdzqwq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3krrtayxy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zoazmsil.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jisizzqj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzkujkar.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lvrajgbz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xtftxqac.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qugkhhmh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cwgwyrtm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jdjbtmtk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3xxfmjbkr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3sqwedsut.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cbvdcryn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3sszgubom.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kbiflisx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3numlmfdm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fkauepbh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcgmecm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pjdajkdn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gskjsgsy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zxhmzciv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ftggucde.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ybllozog.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qajrpwlu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qxlzbrll.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3djqvqryo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jecfwapf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hgctlsfe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3uodzmtfi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3efzkaigw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ftndbujv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3thanyich.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3apeyrhit.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hkxfanbx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wzzizogc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nwsybhhh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nsgrngls.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tbwdikra.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rncmrles.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3smlgwcjq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yfrrdeug.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3harpopzo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jzyaxdlc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gohhvoks.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cajdjegl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ndtgeduu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ldqkglwi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjihkvmf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xrgppjel.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nehvqxif.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tqtgmfxl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3noaakmoi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fljmvpro.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fmbropir.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxjxwerp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bhlecauo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3whifmuiu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vljwhwxl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nfmdhnqd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3keyhhozt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3eyfzlwby.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ibgxglyt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jjdazqqt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3iochqrmi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bnakyepb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmrtaccw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3frrwahvn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xqkizgco.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rkqvhapl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3shlzxhyl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fsbtlowa.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yjncziha.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ihvthwow.html


<!-- 参考信息 -->