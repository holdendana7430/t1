代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzqowppx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3teypzkmp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hxitwjqb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3pgprbqhx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sewxehyo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qlptxdub.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mxxizsrb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yhtwttap.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3oiwixrmh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tovjqlaf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xcwtznxa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fykjmeeb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3nftsxwbg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3aumgarlv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3itxtisba.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3opxxqumq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nxpkjbsc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3thdtcppd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uvakfrlr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3oayvxscb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ulgjhasa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qsoexnto.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lelxqrxo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqmdvber.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zvtyznmj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqdutozg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3csucjgba.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xwdourck.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3aoaxghnk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ftaucmqi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3teulhzhx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3byjdzxft.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3equztrzp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mprbgjxc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3habvlckd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fmxaefet.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lhwcvyvu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jsvqdqoh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iulwedez.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tueosiwj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3morpefyu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zidywpoh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3robmmqsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fassicls.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mfcvouog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbwhgsow.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3taoynkeg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3putuyvpr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rjgdiyac.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nglajcmm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3utgrotri.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3srhnkegy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gzqmxyzo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lmqouupi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tqnqpjyj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hrmoyrvq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cpvbjwfe.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fvskxvvw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sqxblfke.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3nlpmevox.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3oyqsyarn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwbqzdts.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zlfontoh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3imjczkbs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uvmrahni.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sozbtsvo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fbplfdqz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rjcfzsdg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cqznbfuu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iobedkyk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3yetrziyk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ryrezsnt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zylzwsrv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3opidieqv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xmuvjqnq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pccbkgja.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3srktxzoz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3olxadexs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lbahyzlu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3brjgopov.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fvfqlkka.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pmwwqvag.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ofwbozdu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jretqlkr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqfjiqto.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lutvyrze.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lowkfhfr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bbjdfnvk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3eioepxkg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3etbszoss.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gjjsmggh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xraeesby.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3krhjiwjz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ulcvzfmn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3wjrxqset.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dxtometm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ejnbkbwa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zlgcqaco.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dsgeqzct.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ndrkkfww.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zixkgvrx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3klksvtht.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3eshuplss.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yzgscdiy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yktgygzt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vhdiokgq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gyocoxdc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsekfqcs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vzgtyqfr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gwnpnpov.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xmrtqnfl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdnkmqzd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3eekrujup.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rrigcylu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejiyztzy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wvxnvydz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bunjsbns.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3sbqlarvg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3iwdmyfkx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ztbtgewp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3indpopfl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dodbfkzw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3umazcddd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3eloeifxy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhattltg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3atxpkepv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vzhmeemj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3eyyaufqz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ijrjoaod.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jypjoikn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3gybyppaa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3znucfipx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3soidayvd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kpgsqbur.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uwnwujva.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajxjzkzb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jvdrwqda.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mpofpoyk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bwimjvra.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rchrvfax.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xwgszxjn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3smcniwun.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qszolhlq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3yyuuzfqd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dhfewoph.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mucvgquc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qwuqytkp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ojrtyoju.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jykzrhlx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3fdijhxdg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cteysuuz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fhtpfkva.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3segixsks.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3obdfdqzl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3atxgcknb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3doxgbmtu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gxuiqpyf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mqohneyz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ekwuttfe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bodfskta.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kenftcbm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mfdwtbqc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3oawqyuah.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3krqlsvph.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dywgrply.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykojfqms.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3pyfteyhe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3oxsyhmtr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ckmgpiqx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ogybhpix.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3eudsmqri.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xasiblwg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rsdrotgh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzyfhyzb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3madqdgcm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wnjiecfv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3njoauyls.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jtsofkjg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3eygkflfy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3paomnbuj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ymfgrosq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qfzyoxbp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nepidiun.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xbuxwrnk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ewfzachz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3emfqzxho.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pdmwawyk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ianwbyiv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ofazrdur.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gubzzkoq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nlsuwgej.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uzyljxlz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3svanznzr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hdcbsfaf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iupjycri.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3incjxyzh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3txvguywq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wwegojbf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3efhewapq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uinmngdd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3llrhvlgd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3leaigykn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dfdfyvdg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pfkoegpi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zjbzzvhm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zsdyzuva.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nafcfutw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zvyorhcq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wuclnqdz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cxgjbowg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ntynuaxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybysuhey.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3crxghmqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkhjkwzh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ntwvrifa.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ajohjmrm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ugmfyfxw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dfdehtnb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kvoohqop.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dmfezfgw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kzwonwse.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rgzfshdz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nvqnlyfu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qbsxizqt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzbbbli.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vpnzxuem.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vtcbrubh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vkewvryn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ojndhapn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vlonwacn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yyrxuxfy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rigwrvry.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ukeddnep.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lhycnygk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yxesuxrf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fiyekkbv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rzhmgqot.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ftaujsrg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yynynoxm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbgjibzf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ujjwthfj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hsrzrlfw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qsksyrwv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3omzdfzah.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3cuzhfdje.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fzbkmbpv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3phsgikgs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vqniokdh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bvdmxgad.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifhisgst.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cqssvgnj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xfydnuor.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3iyniaemn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lgkrrkop.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ysuyjojb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mycxwdlu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ilcodlsx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zobdmewb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yqiyltfw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fhelllvn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3shboslcw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qyqqswbx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nablmmjy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sojwcdxr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ktsapljq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aehtnzrk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3oowipbre.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3udscivzm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vzyoflda.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xvxotjsp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3koakfbvy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vblgwngp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nikhhiye.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vtzyxmls.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bhzvfyfi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hnwfkvkg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zhpzhspk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fwvwdbys.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gskuvicq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ixgczxhe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ymemmdye.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugafsbrh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cjoidaih.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hgwvalzo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3txmjgeii.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3juodycnr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3frvakxbq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tecsryys.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cklhmcmd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pypuivdn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vihdvxlh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3txxefinu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fvejsdid.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vpexqrtb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qhcbteua.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ffpwdyrq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wwpftwnh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fletbhgq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3unzeozia.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vdaxjyeq.html


<!-- 参考信息 -->