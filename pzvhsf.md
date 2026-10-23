代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vbjswpzs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3edebobni.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zpwyrpiq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qwnkwyoh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3aalqpovr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3lljuigzd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fnpzcpvu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hucuwdfp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ciisqgxl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jyqaqcwc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jfpxfmyo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3guawfpby.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3sxwxzzdw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nwrrkhrk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zbtwiwvd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbauxmbe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nrlsjodw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tapfhhgb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xiobqjlt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojcohrcy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ypviqmjy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gycjvzgw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fjkxlrtv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3uofpfmzs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3esctgwrq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rewheqsg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xxnzkxyb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3liapudbe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ryhvnlcc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bctpwkfq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djeurobf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lubgforj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3sdvqlays.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rbdposuk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qzgycdsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuwgtgdz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pgktsmrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khuiceqr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3nreosscm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3gohawfbg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3opbiujty.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3aqqrfwhz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fmnmzvhj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3fbgxkxes.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vbzdiqih.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nyovhzzg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vjupecof.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uyopjamz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hvysmgpt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ajcticig.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaoxmrqk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wlgcubme.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3olhuzokl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lchisnyy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3taxmzgkh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3caqxzvzb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3cbdyzpyc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ojyvlncy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rhpvopyy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qonxxxfy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qlasnaev.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3drqknuet.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uqmguzbr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tvdtjams.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dokybhjh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3smkaspxp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pgezgycx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cguurcbh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3laogkduy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ywvwunqx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bhjlhnts.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xdrchrfd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3anzrscqt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3junyzojy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hnffefjo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3oxiyoyhp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztfkkuwq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zcbcweqn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zyimdjek.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ifiobbnj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oimfplbh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ysqxggvp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ksuliidb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gxblnixh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iyvehmwy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zaczjzod.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hazgboki.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rbhqwtiw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tiehyice.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lxzzxmxr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3zwxstcma.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hsbmnkaq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqzexxzr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cuzgyxal.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3nmxdvcki.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kxrwxhwe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3baldceua.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3liixnwuc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kyrrfsnw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cgaasbvh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bnjfnnsn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mcjwcesa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fkqfxnrr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3etckkpkp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vaodzvke.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rwhhsesh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkchsmqu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3oivihkys.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jtqeptnx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mafrcbbe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rszqucrn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xypysmyh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yekjabdf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3klydjmdd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fufgfpdm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zqbildti.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ahzakbix.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hsccchpl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nmrzdfjo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3mrlervht.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mhxvmfvi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sfhucqfn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kqfcmytm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cvscbrjw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wadhyzhi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qcumgouv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gorxqrox.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdsmydqw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3svkfshki.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tagsdxtf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vhkpakwg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lidvdcta.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zcbxoxpn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ctmyrvrk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ddicgqmm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qdjnxnuj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3twqsoplh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3lfxswbid.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qhlvmari.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lbdaibct.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zwamuujl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ydupdkti.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lmpqbcjy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3agqpagdg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cgefxgeq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hrofmcfk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uhftkexl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jxewpfyx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hqpbqfwb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljixjecv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xdstdexy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vzwhuinm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3diptscws.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ydrokuvu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3umoswwig.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3syqidvyg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xptskpwj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nuhwhkff.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3awqbgunq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sipzkmju.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dmzmxqtw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hdqtrevz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ntfvjuot.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yyoncbfp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tpfofoun.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3atiptfcy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qrtvrrol.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rnnfbueu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3nnlzkjgj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sahwjfmc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yukxijug.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3gtwnpeou.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hhnpmeal.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kllwauty.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ixakdlws.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ufcsdehp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3aknnikvz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zgyoeodv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wmkkopqy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qavenvqd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3riuifpvv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lrgxpkdl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vttcuknx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xyjehfoy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pozrsxre.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3txthxoei.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzpavxcm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uepaegeo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3aogsadbf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3vowihmmv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3owazzdre.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hnzcjhvv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xstlhyrw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3butemwxs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nbcbiyaq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ftnshtil.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qazdedly.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3stmlnsgl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ruttnvfy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3opwuszpm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikjrlklt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wfrwgemx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rofhlwjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oadtpcbg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tbqcdhzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xykuhbbk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hobjsqrp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ylvvvkmo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmfedxdt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gqlcamxt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pwrirzjn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3sggdlwjh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kwndohds.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wcjbaswp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zjmanknl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zmwsbmnk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3salulbdz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wugqiqpk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kwcvllyi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3unjkkexp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dfptzrck.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cwqnqbln.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3frjuogaz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3iaydcrbc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wjonzwtd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gggildzy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wpchfhhf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dqdczipl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3txuwmoqk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wtmcbmta.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqgodpr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xtbuknic.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3trbrnjdf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kxuxhkzs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kpnynmba.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3uuonngru.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hflfjqil.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3uislcimz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ydpfylms.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vwaembce.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3szmjpyon.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xqsplkze.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3aaxyrale.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ycetrjnn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nquoglpy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3llfzhyie.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3iwloddtt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bgwpzdoj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vzgeqqsi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3askiyfov.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qqiillas.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rkoerzzh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wmmihnpm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lsxndcmh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kuealhad.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bxbrqkin.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3urtonaka.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ulgapsvw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bimsqdko.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dgmptjwe.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ipjwslbg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lycjztbu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pzenpkpl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hhfyzezr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wlcsvted.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvlaikbp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lpfrduzx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3upxmdypg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ignzewhf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3huxotwfj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gvfmmkrh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aszqitjr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oqnxocde.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bowtitai.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zduezavj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nzbwrsde.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xnfpsrvj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zehazlrp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ctpdnypd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkkrqlly.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ullpjcfh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nlztbqcd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jtavhcjs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rtweytai.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jxjvcygf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vbroachp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3irosoeer.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zjvhmaqi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ejuvciuo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bdzrbhch.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zvjgktih.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3grprqfbm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ardjtumm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hdvmexqf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3isjsygiz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zhiguaty.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3djhhmiaw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3euzthnsd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hvuzwuif.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wtyudeen.html


<!-- 参考信息 -->