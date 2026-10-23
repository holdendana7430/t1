代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfojiucc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3aonjjbfu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3knriiynd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ceofsrcm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3abpvjqje.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hcuypkoc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tepgmijt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ntpekqjb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qdfnubpy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hskbvjqk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ubruomrg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mqqfgopi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qjegzhrn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qgyameqb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3scewdqla.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3elnuaykv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dsybspab.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vrmzqxuq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mvmuyrjv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ukqoouyt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3eijzyaxm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vkjzzhbn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jqkyzwoo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3prllgctp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dlvhozep.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylwblciv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ukpqezxy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywoywvuq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3kzqiggfq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qtcvkfeo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3tnslpptb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dindmttc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3foxevyvf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qdhnzacx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3odfvhycp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jcwqndhx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ipgohcbd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tdrzppsu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vgcolsff.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cutgvgwz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3udwnzuoz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rsellnax.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lmnpdtjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxwyzuuw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pbmlpiaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdnrijeu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jryhdwdy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cvskbczm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qloadpkj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ocnjuzsk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ssydmxjv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kbukvvzp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hrevnohg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xgounbdc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rgsgdsmq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wsuahrnn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uckmlsgs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3prdzbjoc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jrmxeteu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqkjwkpn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sdjpohqu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjximokk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tqwzroic.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3plycchyz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qyoxmlax.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3byhqkatk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mggmbkwc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ldnkdozf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3agqnitcn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vdrmfskr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nnlrjnrv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iqafudmn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ppmqhdln.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxckfygy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gcnetdzj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3penwhscc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3aosadzgz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jjsrkhor.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rzdidxus.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fktvzhtz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jmaryacn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nluptkwd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jpshuafi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vjlzeyph.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xcflzvkk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3yljvablx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pultrjpq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3aeqqjehe.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lcfwmxrk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ppzsnrwl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rczokios.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3usrxvmha.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3cvdnzjrl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mugjsjle.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hkqbfdpj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uchcqdtz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bhsqgfbj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hrydilza.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vypyoret.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hdziomwd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3gkhlkfvu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wtpmxger.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vzpwpbey.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mvxlkwoe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nqwvflty.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3olnxrwjp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zkycxdap.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qpzafyjo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jkrmxwgi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zvobpxzz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gtnegpbu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qeyyntmj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrqgnlox.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3iogqgtxf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3efxbjvhf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3iypfvyvh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tvhcbfsn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nvlexnli.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ebcggpat.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cfiyjkfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jsmewtdh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bwgsdoht.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ypxpeifk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gidncbru.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcsspfk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3oudruphc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jivjnbwf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3czvdjxdv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zajanhmh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3iexctufs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3upmdnqna.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ciredsev.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mwsfjfzw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tronryzj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jsrnhzbt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vbdlxioq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zjlgoeuh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lymoyglz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mlbgsscl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fmvgpipt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dbimockh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3mhyyckrg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lgxgqivu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3oldttsid.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jiomhhht.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3otjbcbxf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xuvygrzs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wjbdpkle.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kfuezwkb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jpzwhntn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hesdxdpp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bmvfgnuk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uyrkotij.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xbbepqol.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gbugmffx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uyozfezo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xtehtufl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnzxyymg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lnjggfmm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yafftwla.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ejcnkuke.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mfpwvdsn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3iqhfyddh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gbyjfewo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dxhewtpm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3srqtzkdu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rppqhhls.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3brhfqeai.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xxwjwcfw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ypounlir.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ghwgjbtl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ftxiqmeu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kvsihvpi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xuaiftuy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3yqguixhp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3waufkpty.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uwxdtcwl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xxmelrvd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3htathvfv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3shlwcvkd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3knfmyanl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xagxktas.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3glrzeazj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rsvgwquu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vuwgrcvd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vjnwcncv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pewtfqtd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nworgfbd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ezxqrucp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3loikpzne.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jxypbozq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ulmslrly.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yskuessa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3khxqjcxg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nrpolzzg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3miufjenk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ssfrpuap.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eqjvrksm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3othcjyrd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kardwlom.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3oymoaqjh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rcsvneqy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rinctgvm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vjknursn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ihzdcwsy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3agqgrjia.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cdudarfc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qyioyhwo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rfdwakbf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3eliesmfn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bkekdjnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygajedmk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3sxsexlim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwogaamu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3imicsizm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gnodjgyc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwmrebdx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3htbkqfxs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cdgeliqg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3flrcpdir.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ydpchaac.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dpiqvpjb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fyfphwoy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dkyhdcwv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3flynayxo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ezmmnbjs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jwftifkj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xgqvpfus.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nmaufzau.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wubivyte.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3cbbqkgcf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3smsrmzqk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qgviiujj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3khfrfnwf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dhbsxjbq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fuodjdle.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xurvjlbs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vbiqdjhs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ijzoseyx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3eswcebdx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3muqgdett.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nqqmyiho.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mwwafdsx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vfsgyadz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rwtgjoya.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tstiftkv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3binszeuq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bpnbgrnx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iqajoycr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gedyrbsh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3czdccfje.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3slqomklf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vaauuugm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kndmpego.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uiyimwes.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3skcpnqyn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tqatxvgx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xhitzngv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3euothueq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kkfrjbkm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vcjknpgo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3toqqfupq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3xyqshwra.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3liwdxlby.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ciugccix.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gprkrtlz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ztadderh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3uwktyqoa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3swbvyuyg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xtarzszx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fdxnospk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zvkikexh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3juqrshey.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqemykos.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bolwxnqh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3spkumjxo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3injuwtgi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3pzovvqpk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wfduvmxh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pfembomp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ilhmqnyg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnodznts.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3awlutlhc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3bigntadj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kijjvzcw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jdbyneea.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3cvkpjfym.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vtytrmeq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3apsfdvzr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gfbmenjq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nlwpwvmy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3byqzewzv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3slhbuash.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3quqgewdy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bpwtigef.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3obmbqprr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3iaotogim.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pmarlzhu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ddjseerg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ywxrdyzx.html


<!-- 参考信息 -->