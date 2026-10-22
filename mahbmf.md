代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2chfuxlyk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2islzipjm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zoodigbf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bnvdeydv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vtlhmcjx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2uyrqqsyd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vpgczpez.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ekvkeiwr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jsgzaddx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shxizcyq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2reghyqdh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aspxpszi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2eykqwzgx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdiygzyv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uajhpkzj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ylpnxqjl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zbtekfnr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xboslsly.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ygdvjctj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jlmuidbq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2osmggpvr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2sjgjcktj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2byqsqsbj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pniphjqw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tvzkocmc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zqwxqaks.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xggrauzf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cnyrmnap.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cragdixl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xxdmplit.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2lmqksbzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqtdvpve.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qrvjonjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyrqglly.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2oduifaga.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2exryrslk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hidbisbb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qbijpzpg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vhlwqrhq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2kfucfvbd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zuibxmky.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dovxcxdr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cradextp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eyykubcm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2aidjurvu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jhmnihrt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzsjiwfc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lbscggiv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2plbabrrk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yxcejssp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uiocldja.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uzwerqfz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qmzxovxu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mswtwazf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2clcidmgv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2frdjlhqn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2lzlkylwp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2scoldbht.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kpukcntw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2sjxvqhch.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2padnqmmr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cudduqml.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2eetxcerm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zlrmatwk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jxnpbldv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ssluuagi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xcmldraj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlcqlxrc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uzngljlj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bselbytk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xaxhqhyk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zruniyxi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iuytkasu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jzfhondo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwvognle.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2aimhjrfc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmyvetzn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2cbmpaipx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yghazrmm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ylacbkru.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ekvoevus.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mcpmyzpw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qgefisjo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2skstarrw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2curodjjp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lthqutmi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2elzolikn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tkqbmbhn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fxpmvbnb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2phflqizy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2tfwiyaxl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kqlmlaxj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2skiadott.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wopgjgil.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wkazjabj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2odtmqqfz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jrlhdhtg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kppctphh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2drihyswl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hbrhboxm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozbvljjp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gheymucm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uzcvbzhj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pjrbnswu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2szscunir.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xysbpxcg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jndkzkwe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tkpqopyn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wjrxuhvz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rzygnyow.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jzenblsg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rlrqtfex.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lxqcjyhu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pypmeoia.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2feewrczj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cyvtuskx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rucrpwvu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2xecznqxn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2suzlvupy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jvlrhqgb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tcaloitt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2eaunquvc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2glrgpsra.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mcepweyv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kgiljqkm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fwaalvpf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cvbykbga.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2crvihiax.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xdfasnsy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bkaodtrg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mzmuvjlb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2snnajgwr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xtpkwkiz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2enzzhzos.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wstgfxnz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ufixhido.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ruelpwne.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dbodotqj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cgturehn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hhnthscf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sisyydca.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ibyemkpj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wgpxglib.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zldadyfq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2chptfjpl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2udgalsaw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dzrpkchj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mislwqvt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ssrzyxoe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qdpndsbf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2uhsjbtri.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rdlzhboo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fnfqdiay.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vncehisv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zwzxfmoh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bctusbdf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2usnonzdu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sqwwwtff.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cjfoohvp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2dfvdpwoz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ufswxacj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lmstnlde.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fhabyecy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pnhxhhuj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xveswduy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zywwpdox.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ohzlevey.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2oljbfgau.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2obymmakv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2arpwzalf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xristqtz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2erbguaev.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mswaasdw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mevrdxop.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2svtuavha.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oleqfpbj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wcsbvqwy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hrnmmnev.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zriipogq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ctebxyhd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xrxogtrz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2chuzgzoq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tjeghvuo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xeidxdpx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bftcwggs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vypuapmu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2opidpdza.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lpflaidn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cebdvnxm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vpmzojvj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bftvudkh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ncxpwwyx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sooqsczq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2invdazwg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2czxmiggw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pqkuercn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2elbpiucw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ogcoxqog.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gpneogha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leotxubb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gmmkqojr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkoufmrh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nuhonbjp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mikpvwpd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrrmqgrt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2eduoncwq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gbmqyngc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fomquuvw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ohuqxgum.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uzwzefme.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gzaidyhf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2niovmhsc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2cmjtbqee.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2okkfoyzg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tyxcpjlz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gkochxgy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hkjhpayt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zdhyudjo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zrwcsltu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kqoapeiq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gnqnvpmr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vsvnvvuk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lltvbnxp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rsjxutwk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wgqrmptt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cyhuxfik.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2krgmyhcz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkirifds.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fqvwufwl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kxbpsfog.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ojypzedj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nthtuxff.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yhzxmeuc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rbwvyxky.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fiztwxyw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xileoziu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fkvrshmv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qihisqqg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ueckwkjk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yzfmhsmw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kvivioiu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qpuzieay.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wjilpzgc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hgdkavet.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ulaektdm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kqslvcuy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nybtsfir.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fodemqcq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ydwoycqa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dlffltxu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hkygdovv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2khqngijx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gewuxwlo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tqerdanj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2frxfptug.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nivystnm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tutbwofu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vhtkjwke.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2khfkhojr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kbthcbcc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ylbqwkwb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uzmvltxl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qilzvnou.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ifpqewxk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yymhaxpf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kruuxvfq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2titgbzel.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uerjxbqv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bnxaazxz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldozbvmv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wpdomyma.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qzjlrwjw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bmqljmft.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2niktthle.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sxdqbrlp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gbpanxdp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yydzvvml.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2riutqbbh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fwdwfyfw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uykfedtv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zmechidr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ugookdzq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fjckdpiu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sbsamajy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kfbfabra.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2selmoiux.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zlbyaxsd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tedejwjb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2anyrimnb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qlfcpghe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2apkiqnvu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dtahictl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kouybyza.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2oorequox.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2deuihpaf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2boqhzyaj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2adjrilyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vnqqsjqw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dnlvxrtg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2yexthyko.html


<!-- 参考信息 -->