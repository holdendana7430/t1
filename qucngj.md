代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pjgzcoih.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3shwnvnwv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jezzknel.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ldhlxhmi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zcwwmufl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3uvgybiju.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xxotvycj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dnnzjgog.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qkksftzq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3yhcjhyue.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ieotcyab.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gimpqlrv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3drwhkkpa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3behbtlvc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pzzhbxwn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pecynlwp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pelmzoud.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqalafqy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xcuppewc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3teigtwat.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qlrmlldf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hkqirgnv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dsimxtng.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3aggjjlnh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tkjhwzhz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3dwipdrxy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bpoltsdg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gdludxrw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hxqfbezo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zlswifkg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjkfoafx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ttytnvxz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lejfwigh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ajgabcou.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dijstahk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbbuoesx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nqhhbwne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxbiceyv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3olgjnxtl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3fxjcogyb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3dnzokrkb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wkskwejs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lqlpcsya.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvthpjax.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qcthogxz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kngzrijy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3snuacbvx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ujhcoftw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fbabshoa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lwsysxtu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wegapgnt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zrbnfwjj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3goteipoj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pvfeciiu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xjfebdtr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dqbijfeq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nhqupodl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aaexkmnc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ztlomckl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3fvjrajih.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zqvjbbyj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zgbcfrpg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wbjdknsg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gowqdjgg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3yblubizm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3edhihnan.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3psnejflc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vulnreht.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3moyxfkrt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qpbkycoy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3enxmlakp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nxtsuuff.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qeeuycpg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mnaovjyz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iaguxtgv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mblycdhk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bfoaytwb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qusplvdy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3oetoervz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jlfvzoyr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3esqdydjw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3iqttwlfa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bjumbyiz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vpflghrl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bwqsykkb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ivmpfdvf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3keutlryu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3udbtrvrc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wzoswste.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtsvmjlr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3obckgzks.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kzbvykew.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wrugntqu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qfjdzaxs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3csuedhcw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pivaqucj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wnoubars.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vftynxau.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ebedgdiz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3oajzibwq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wcgklnvw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aivslddx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xugkmkxv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jpqucvpb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qozpxwzm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rowjxvmp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3czbelbqf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kqlflgcb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yeidjhim.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ygwxpwnn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wjmvmrfk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fxbpkwpi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ludhxdxq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cbazyiwr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nrilemdd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dwmedpdq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyohsbxy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lbwamucj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xnnngjwc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qkcagnvp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lzwrhrjj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3davaegww.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zzmcqhnh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gcwqzytn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tlcrnfyb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rdlqdwms.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pastpyau.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pbcwivvf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3flolajls.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3evvefhqp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rrlmxemf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nhniokbm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rapfbhyd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ddtwhnop.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zdxxjwhz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejrxwefx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zlpnakmh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fbtnwbeq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gbotuqav.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gddgwpor.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3glzwsczx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pbojznco.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3adkpdgmo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uanhbsmw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3blanogli.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tmwqgcvw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uixiekpp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nuwgdetv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mhwzucco.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hnhbjmjm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uevrqvfh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fpkydbcm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3blhluncv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aaqjprsf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rinnppsi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bzfzfehz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iipkyxbx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3clonumxb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3siwcyhcd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lgrrhvcw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3txivufgu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uxdsntvj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xwyycjfv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zucgdlkr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ksmcktsf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkgpngel.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3klnnfumw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lzcxnqxi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3inaeiyps.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fnnwwrgk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3iwbvcrlv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3sfticlba.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bxixvkpq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vuyndpuz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wmrtxsax.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nvxrntxm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wnoeocmi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jvipglqo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fnjvnwzo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wjpvoyes.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gplbeyuh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3soqvbknm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ojdtiujt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wlhhlwzp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jfpsnhyw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uzzbwlfx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hzqubfur.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rqbnahdc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bksnprjw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cpfqaoju.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jpspfomn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vwhqcpav.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ylgmftgd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tzfdloxv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cjpovrgm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3rajrljzi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pqdxhfwn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3oskjxafe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jeqrzbsf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jorogavy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dbaciruv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rsiebjdz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3megsgwpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpiicbof.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gcsrjwjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otjcdfif.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jsgxalmv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3enpwlioh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3uhbkvrvh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bcuertkb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3oowcnnig.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qebhzcbi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3osvmkule.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3kcialmjh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fdctcmqa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3akzblxgo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nbavgufh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tgvjralg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3gdgpuipu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3menohdwh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uixaokjh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3whpvzenb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yijomjxu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pcqinpjw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rtordill.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pjnxbhbx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fvjrzphn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixbxlfls.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xtvocfpu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3putzwrha.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pgkgpgwt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3czrvbzzt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vlwrfakv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cvktnefg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mzvoqfay.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vtkfhebs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3deofytci.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yhyeucav.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ekzqqxfg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3corynwon.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pjoxarit.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpjxyxda.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3paxwiblb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3amrpdcpi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3umpbfitf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kejsawsp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3merkqyor.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hdpzqsor.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yksstuse.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3eutkvtqo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3otgffjrm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yegbffoj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wliysfqb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jrlpoboo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vbgtyyig.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pmranzea.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wqtefudt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qfoagvkl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3byspqedo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3iuwlexej.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3pfasuknr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vsupfrmw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fbzinwvz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yqafpafi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3shhoyxvx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hyoerdbj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tftmlzft.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3flygdipb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rwxlqmyo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3czoiutup.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ouromnov.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rwzgdxkt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qlpvwnrl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cuwjvaqc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lowcuelv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tjdhqojt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dcgzroyt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yvxsbsyc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lekuhokj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rnspnxmm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3klfnpizq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3amcxtybk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fptoothd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xfhlzite.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ierbneuo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zdquvbqp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3exgwimnp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rtezpwgv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wadlegun.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3oldfjlcx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wearafcs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zfwcxxtf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ryjvriun.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kbdqfrcx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ugimzqgt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ltdnfclg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mckzcclx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qxmajjhf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tiopesdi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgightdk.html


<!-- 参考信息 -->