代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3sxyrwtwg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3junlfsjq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3weyaewhz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3eevzgztv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hgqfsgoy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dqdexbun.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qcmzxwhh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ahaaxiba.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wamlxkyk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldtqhfdt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ekkfqcfd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yxwhxyos.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zidkdnqy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rpofhgsm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mubnrxha.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3auggyrvx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ybgjqucv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dtbmkyls.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3sbzgnkxz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hfqnnejg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fpivlqwl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jtyuibea.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tmgyqojb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pxwjucly.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ztmyjlcf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ygfibrkt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oiixqwfv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rydihndq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3cecfaeju.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mblltpgo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yxfsvfyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umxcqcff.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hlernoyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lleghfue.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ynwujfnw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3evtpshnu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cczrigbp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ezbakqwo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ehdcegyw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3iodprigl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3nicdpeko.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifwkwvbj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ddxnyheg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rqrygtob.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3obicakjf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wbylnrqf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3izjluwzj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qowhvnry.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ddyyqccw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgbiuhec.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3cjwfadkf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3atytlqcl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bwboqzfe.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3pofdftmo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ddomvhpz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gijmxmpy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pxiciqlv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3igzbvdnv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uoaklydd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3uahvpkuq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hgzjqviv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrqmslxe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ywzmnamu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kgyuaohb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3omtdazfg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3debhxfdq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3btmzeowx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wttpdmad.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fmhdgngn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ixtnoydg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tqshtfwe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ndtlmhrh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wotutnek.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kmmckmdp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fizkoiwk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3owgcgith.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jrdkeuhy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3kuszdecz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3iravtacd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zurkefyi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wxotepas.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3anzavwkm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lgzztwsw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojlkqeth.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gdojdljr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ucxagwli.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wzcgmotp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fnnlndrs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3oisjkynx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lnaqqlbi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ikpkvtkv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qquktvko.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jldaxdwm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sjpwwshq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3scauygof.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fqhzayhw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3aetjhhrf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tudxypxx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nujsbwtk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kymxtmib.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwukzinm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gvyrgbbc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ysphasfx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vvfuvinw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3oxeymyuh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cftbaefq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lfcyfnog.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3clxndwgf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mkacqhvf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qmurnujy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pmjpwdkw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kkgqaewd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksagatyg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cybcyokv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ufeoapvi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dvrtjarm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tycypinl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3nvleucxy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3efxiiwkv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wjwpefhu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ovwswqtg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zqnxzdrj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oyrfglie.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3kxzyogxz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3iaasktkd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pjtjtvav.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lblafbgk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3cutpzxvb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bfizqmpv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zkdbktwg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3afdjrkxj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3plnojhnd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3shviqzde.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qdupkhgh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ohxywfsw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hctacnna.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lbohudyc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3yxtsktpo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hvjjprho.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bicrfghq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xxnrmkuq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3eiybewha.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3otzhmggs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gknzljkw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zfpbtnaf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uuaiptka.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pwlmzofa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zmsrqszn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3patnggrm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fmfseqla.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3fycvoezk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ajrwcnsm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ilnspiso.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dqsqlthc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3cydlxzzw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fbbpvjsq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tzhhhahq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iarqgldq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3yqivglby.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jrllmlsx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ozrbhufn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnxudlnk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ciebsbkk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3almvmlpa.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fkoemapm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3btauyirj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3alpisnbf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3roqriobo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qbfoeofd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fovxspyg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3xsadceew.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vmnrbjoz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rdwccjbw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3muinkxde.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gbjztcka.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rsxyrgym.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bjvfoefd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3blkivvrt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3urkayqqk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aatjibnj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ipolvgzp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zwdkfrfh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3unqqimsn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zonsnqes.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mprerosn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3neaiqhec.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hqzjhscl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3voucxyyt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nvfzfwkv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qsvgswza.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eptkvaea.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3coztxkfn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3brnilhfd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fmxeszhy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dduhhyip.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ejerqntz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fiipoezl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3evgonoqd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3deuqbenj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvfwkryx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rowtjqul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rauiacbe.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3llgwmxnc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3adaddpge.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3eianuxbb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3icfgzafi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ghsjeipa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3eoobwstl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lzvsftcl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ckvcosjz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wjieievq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sgswvxvf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3sobajbup.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gwdphtog.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3enggtcxv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rtsucxlo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3czowuhcy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ggxkkidd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xuzkypnk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3claovhnv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hkonhpft.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xrsfiphb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fqdpjkrc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qurlijzy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vdyywzqo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3elfcdolz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cyojnjml.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tucawdss.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wadtwamo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lgolvdpw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ptshbtrd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kmcwzbsq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vohzuifg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qjfkgzjc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3scbndyui.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hxmnuwhz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3grbsvxlm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lalhqtjb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fwpifdre.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uyqbpwxm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ziqdexzm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lwgbhjnv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nonrlygk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fhefmpgs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dfulxsve.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qsxyclok.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jmekzqsk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3offapfnh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xnerdyim.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zbjajwfq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hftacwxc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3apemrkcy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3emxnauqx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ybmpvyxt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hhoxqhci.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3arotdcja.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3twcvehvk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hfyafwxc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lvlewcqs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zpkdiqkp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eszkjwln.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjfveapa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zrlkuqzx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dqerssjr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rhczlegr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dvbbdszn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hjqjmwfl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nhzmoazz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3satdjgnu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oybwitmv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3aysmqubv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3sazaxpcs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3suulzhpr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3eknevpck.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3uhhanerd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlgnjwty.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qkclcnak.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oaygsgis.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bdyzuvqh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fylkkewa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gaafxyzg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bmkxfcig.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3womrjaic.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lphfhynb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dwfjbroi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hstljfoh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vetzufbf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3seljghhw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjglqitn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ovofplgd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lomgqapk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dndprjda.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3akmgfmkn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yjkuhnwo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yiuarcux.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3imapqngc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bljlctcs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3drvaynjt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ciwygeal.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxfmiuna.html


<!-- 参考信息 -->