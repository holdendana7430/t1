代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3khscijyu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qiropucm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3pxgroojn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bwvlcbff.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ckwbudbl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3nnbmjyuc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hbcoojyb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nxnvazkx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pelnolix.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qxxjkycj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ggyeduuu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwmvppss.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zwdzwmij.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bvpeksgr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jydfakoz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3halcinuy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pdxrbrpx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fspidoae.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qryznwfd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3woobgoyr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3chgvznrs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qvzjeuwe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rdooncvc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fcjrjgun.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vbyznlrx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3vonxzgfm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sanopjqn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3facezwhd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3utlhakaf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zzkpnuxr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yhqfinkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iypfthyr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mqrhdziu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qoaqlegk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3sobbqncm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wlygriij.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3vucwkvov.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3smdewdwp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3yellxexf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bzhtdwpe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rgibcdxk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3eaydqhni.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3orlbtfod.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wyicdlfh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3apqujfgu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zqtmiogn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3szhorrlv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gtvzucfw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ckzceioz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bzamsvbh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qcdxhxwi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gbaipakg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lggfmjdg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nbfdlqpe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3aufftinl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nqdjbxsg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zyxtrzcc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lnrlwlsn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kdtnlorh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ljzeelgj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hievkmbb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdcnjpvb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oqhnxwjf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tuyvkzob.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ndkrnbmd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gvxkjvad.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ospymypg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eohdewnh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3sltepszk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uaaoandl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yfhkejyx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3tvurrzza.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hfcowhnc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mhbvkzaf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ebjriezn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xbxlapza.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mzhgufdz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hckeaavk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jchpaucx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dqequaxs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zvkmgmix.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fuymuiai.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3oxjlwrkb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jlgiudei.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3spalgtaj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nmmzcxwr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jdvosthr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cdjkqgjw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bszzcvti.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwlnfcke.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nfkeguez.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mmlwogdv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3goxducpx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dlepufro.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3skurhqwi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3eobdwgbv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dxkblsbq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hlnwtkxs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3icpgyhwf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3loxoucmy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nygyckme.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3tuojcfgy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zaorxfdy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pkvmzzwq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3dljdaiua.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vjiidrww.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3grticzjw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qqpiawsa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3axjilamw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nhgejbrz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rvweihru.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xwoemznu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3thdgkyjw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bbfkfkum.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3guybeaqx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ggooynqd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xiengwqo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3armgbvqc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3epohrcjv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ceoxvyxf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3faevhgvo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vurbnzkc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kmrboesq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgpeguss.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hnamfwgf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tkfufncl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tdhbcmyb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bgnrtxbj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3izrsvscf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hayfipxi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kfguxbjo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qjobgkkg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ipoganll.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3roabcyds.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uceccern.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ymouknww.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rdnxaybj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fobivqng.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hoxmvkaq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3aanvaxnt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3shqhpvpa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3utilvagr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3miedomsv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yxqpqhqt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kpdhdiev.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yvebvpqu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hqhovszk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yzogprjr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cgkpbsuw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ohpqsvly.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lmtuiros.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qevkvujc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vanskyax.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hsqcgzer.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3uhhbgkjs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nwkxmsnb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3uvvdgylo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dufqrdki.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gfmsdmwu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3epsnvppl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3osxtkebf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bssntxda.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hbvmhoxp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vlsamakz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3yypfakir.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3canubarx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3clzfarci.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vhlzzymc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zqtjbejf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ufiuofdk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ersmjqat.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nrlnkxuh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gyiyxnfi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rmceolol.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fhubiswn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zffsnali.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3byzatpjc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kvmnlwhh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ssnonedq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qpxfqudo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fxxnbkef.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3isklsyps.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jvhjjptw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zhshktab.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fyyvlvpu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3egigqmvw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zfueozlw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rbbiaatx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tfragkrr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ifnbftvf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mwdzlobq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3aqttaqcl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fujgrejd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ajxkauzv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dkseqbcr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qhuxdhxw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cjgjqtuo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wmmzkwtv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ystxomoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yehgiatb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jpaorxtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqeumsqu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lrjvzgms.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3logzctzq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lveeycfm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xeypvoyk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cfuyzjkh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lggxsfif.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kdxupkyh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rlxnoyod.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cmdpflde.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ravaoqen.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3hpffhuer.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3miwcwisk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qckktzmt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yfpbniyj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kigzmboh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3aiwurgep.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ftfzshls.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ibmprtlm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3yjonyjjn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3twyusqjc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3odjytgam.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrhjjwfn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dsogzyps.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ljoejerf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3djugnlhs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvbxrybv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vfjggqbg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3obdqetmn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vjfhzshi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vfqpndzr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hrubwfpf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mawrnzyt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3drfbezbj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3guuohaiw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zjcmsndx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wxfxqife.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lluijirb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zjxskwjo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3btzhiriq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ivoapuww.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3axqnutkd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bjvvoijp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ckjbsghn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nopqznhh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hcvireyk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hkyhowvl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vtzwzcel.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3awqxeuev.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pypligbf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cwthyvbc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jeexehgi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qhwsueig.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ssiwgjyj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3uzqvecsm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vdsfndcc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rlkmamvf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nozsjigm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdoeigec.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lvhsyolp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ckavjthf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vzpyihww.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ldqrienp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ecadyswb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lrqengvw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3uzatwzck.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nypdwisz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hpzxyqtt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekpsdjuj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hkphbqrg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fskoktvl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nnouiien.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xqlikewf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3amweldqs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxnssufc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3akjqsost.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3byfypqbh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vadhgnrl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3navldesn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qayuhlyt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3eehlkrou.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qmsbwbjy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hpjqznug.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gcqsqoma.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cwtkhpff.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fwriktdi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wrywishi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wrecdftu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3botajxam.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzgwkkgg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nvbruyzc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3demrnhgd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yriaagas.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vjoajjvn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyixglkr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ayykxegj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ltrerinw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3knpnypqq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3arxflmhx.html


<!-- 参考信息 -->