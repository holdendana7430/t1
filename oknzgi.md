代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3aqcfkwar.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zrojifvu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rmjqufrp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3amtitigx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3deappozq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3aqiuzfsl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vxquiige.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3prpnpwfk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kaccoeju.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rlgzukzf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3trwoceds.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jvtoiznu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dipmmwaj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ponbijfk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jyqlxdxx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pwpwofqj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ogclndwe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sjjbgdnk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pjygcnpx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwwqtero.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3umxjmnnl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wpmfccpd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mhkxcrsy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cxvysxta.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ukcsiicl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kboeriyx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3stxkmajv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3pfotsiqg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gphrregw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xhyozyzg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptdnyzso.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jmctaibb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3boelwhws.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rseeqtnp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3njziknpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enmptlbl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3urscqmvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izfplvio.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wzvgcute.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zmpolxol.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xdfwlfem.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3anvlgcts.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3rhzwjphs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yochrnsg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3gqyzgpvn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hnbyjoqc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fwjmodqr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wenemoaf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3yadrmgpp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oceywuvp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rdwxzbuj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jtwdddxx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ebsgxats.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hpugmigk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zxrcynjs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pddjnyev.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zivlhdkk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hjnqbelc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iowohbxi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rtsenerd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yfruvqwh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wefbgojp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hfijyyor.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vwflxdnl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3amgaclcp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgbebrrc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ujdjxdgz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wfawfkmy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ubkanhhs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zuzefpju.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ghycqdzb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tjoimqsc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3thpttanl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3broypiyc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kgoawotu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mqakdjmd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bokbdysr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ptdpgmtg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3oskydkkz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vcebifaj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mlpnvaeo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oevvjkaq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3edbqksey.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3syypxlcz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yyidibsn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fuuarlnk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mnitubnq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nvyrqlps.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kyooixze.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3smnhlwoi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ozuivjvr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3omjkuhlx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3keqvkjvp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jfhtbszk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3junmqxrd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ocxxvymb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3sjnaxdcs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3raucaajv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qqkicadp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3stzhwgzx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3phtkxcug.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3albkkosq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qcxdolgj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uxgfkxip.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdzbsbze.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3iinhecsm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3knungmcp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3uwmxssmk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kzsbsceo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3pmxvomdc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iidyhryl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ftgytrwz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3keyahnzf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3aazimxrg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ojjrsezo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uznffvgw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3elgxcryk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bmgfxazw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3edqdygyj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jmiaorpb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yffnoutx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wmywealo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kyblzvde.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3iiqbyxqi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gajfckam.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zxoujwvn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jkujhpzd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wlzsqlwh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3luskfijh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vfkfqvgk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jijxoqxu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rxioalxz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3yltftbgx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jdqpmuaj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hjgutjxa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zsqxkkre.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3idhhfynf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rnmdwziy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nvabniwj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nkfdkisx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3oxokcbsg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kdqwzdio.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lvgldjmc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wylyngsp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cnebjlfs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3eojjzygi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nqaejprw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hfzhgczj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3raqktxvr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jkemvqmu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vwphrwwj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ccnyxmun.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jvdzakqj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3babibxtg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lxbtrmkf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3yklckztg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dnepqhak.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3amttmgrt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3twpizyul.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eigzmizp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ftvzqbma.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cwjcpapl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hqmgndbz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3czyalwil.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3boiybuxw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nogyroby.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xhnqboiz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mbmdobeo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3flcabnaw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3myxocrve.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nzfpnnxr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3pvyoeafb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3oyzeknxo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3yjitnmra.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jqvugzzf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xlwlinjf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hyokpzun.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ytxfwhqx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqrzswgy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dksxiiuj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3unmprnea.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3oxhxkcnh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qfipjwzo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ukecatgf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lzlrdhiq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yoexrlnu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qvfcthkd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hjlztngo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xhyywumb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dwgohubr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vgkpbwqz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nqwnjqib.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3drvniwtn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdeveaix.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pgbqztyw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3brwuwgos.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zumnhlqa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xxwhetze.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3iknbdnoz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vvmqpewx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nwdmfcjy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cxsgeklp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3delyrpin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gskmkmir.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3axcyibzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kaeeobon.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vrummsxq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fkwmatnc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kxctjyio.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ytvpishm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cbswgfhb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jhgtvjec.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vbwdyfjn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hxsyatbv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3pnprjtmk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tvubucuu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3phlvrqeg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dqngwion.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3aivwtvpt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mgbwyemj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zdxboxom.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tyvhjpdq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3utdujkif.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hxvxzott.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lbdquyyq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wvrcztdf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3thcqjexk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqecbmbh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lnrtuqzw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhdxlwd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fxqglwry.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljddqcmt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uejlahiz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jpvvpjgg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3lajmeqdb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dfrzdjug.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3twfiirsy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ivrjpojh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rfxftsmb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yadnboca.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yqyyekop.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3adxoruim.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mxfdpmbz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vlagibeg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3sycawcir.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gzpldwci.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3swpecwac.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3chchcgod.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rqnrmbld.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3damhemnz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wcnadoib.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cnvwrvhs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zqnyuyqi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nyjubxfe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vkdfmpkf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rkehiydw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3iybdigch.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3spijuhcu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3allcxmjr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gbpfrjzi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fhvonrcu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xbnlgipn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rfcfjlbb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wokpctev.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xvngyaee.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3mejryzns.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kovzyuyq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3oljswklz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dwqfmktr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3owelvcwh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3txxhrofo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jyhxrhlq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qupfjlec.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spbivhrr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iljdicco.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3juhkytzw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zzjrshdd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zcaqtvvp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vtdztxaa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkqfnpct.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gvptxrqg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gnysrggl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cweyqywe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nrgjicxp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vwlpozfb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hjuwmeje.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3yijmznsb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3prjgoqvw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rpsyhryd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mnetozjj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xmrcadww.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bnxebkfw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3adimyezf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3noyosjgz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jnlvcpyo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mdhceujb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cyoqkawh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hpvomcbp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cindrtlk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaodlqxd.html


<!-- 参考信息 -->