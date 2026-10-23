代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tbogrqym.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3unerabmf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jkrojqcf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tkobnpxp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3elbxucyr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3peezqrny.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wzdxozgh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bxieaqes.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3faohsfhs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kwchbpxu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bjtwlynj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gjwstgic.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3sfxsjybl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fjkerlsx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmigmkai.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zeumqvea.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3tqhcroui.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3tdmxxeuo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3mzyqbwse.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mqezfffe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nrvzipth.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3podeirae.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3msfdmelg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dxdhhlzu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3vwrxkesp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cmkahsiq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3byijzjgu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iraojmhp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3orlmhtgd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oggqcjqo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fvdxdrqe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dmbhawdr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3smkopjws.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mlmcympv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3xszmiash.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xtyutisa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3dcxkbdxk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sgjvbahu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uqnsrioj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3oqpvssqv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3juxvgkqb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uzlkpjjm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hzeibjun.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3yauldbpd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ebbovvsl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3eksqdiyh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ckgstegj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovownwpg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ogggjhis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulhnqedf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iswtqrjs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3njhgphwl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zbaavcqu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3voatpgbz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3htowkadk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3hgkqoppi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3nsmmmcjm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bqiapbwh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3sbimoovj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hlfkpadk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hoqmujtd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qtnlelnz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bktpfcdz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbhsngyv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3crapqdgg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bljqodcn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3egghkjoi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bewuoylq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qeawkdbt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wwigzxuj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ilnflqfn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3iygurayd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3igzfwaow.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wmigvmcf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pgokylad.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3roqzifgb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nxxgaana.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xsxmxoku.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nnrlwqsb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jaqwaszi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ppchyeim.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3oxbuhpme.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kbolfcfs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fclbadff.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hbjrloxi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3sxfihspg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggytkpup.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rhepgozj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kxcqosvr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3gjvgadyo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vzrwhwcr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3njceeelm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3kdeyaonk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3icfcmvbh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hafqmofb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3udornwxc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ppkemdcu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gbbzcgjy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdpsweol.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3edkhujek.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gjvwiybz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dletpzss.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mvvahfir.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kmyefnoi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3sgkmpnqt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vduvfkiu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3frosavtg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ldccklxc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vilpzmqg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3atdlshlb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hgooqger.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmzaiqfh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3uqqlplkb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nvipbtvl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fmdtmzqe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vdqyxtgk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jzqjcpds.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3aauckmko.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulzduxiw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wlxjsfqt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cpwjqvng.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hzzekiri.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fxhtocdg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yoxbtbww.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yisrxbeo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zkdqcxte.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3barqhzpe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dzphrwek.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jccmyyyy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wmxqntbe.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bqjvbvtx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pcblvgeb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3llptcudp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3oagxbcso.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zeesipok.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ideqdnnj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pexxfqwo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3cqgfzzgu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3alyhbdxf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zimvityb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vfdjooeb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3oyiwpgja.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zehbpryb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gskwngpi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gljtfhvy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gzblbdzv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vfwpuktq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ijfembal.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gedyvati.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zwybwrfz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3deytrsng.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qevemikd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wgjiogqc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ojrzriih.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nzkphhte.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rirkxqxp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3edonoooj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3sbnyecdd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wtbguuei.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ntahgrwm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zeckgcrm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zckyknfn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ortjwrsj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3keasmmus.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3unhewrli.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vbzvnsib.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ssokxfzy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hrsclhfe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3brfucknz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3crbkxovd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3akuhguyj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ubbmpjxt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ryeoaeno.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uwadqcrv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wamnawno.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3eznzwjtj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3djtqzzny.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rggzdsmj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hwotlgho.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3oqcwxyvt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rnkopsel.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mntlzkds.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3myjjmkyk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hgneakst.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3snfbtjvk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ekaryszy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pazeuwia.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3iffqlmst.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zhhnhcsx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3verpcavj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zrolborb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3splijxun.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nkdjgiaf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zvowwwbl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3szoywffb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nrhvjbei.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zzqkwksc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3sfovotpv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pkrjyzxw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ubtmsgpn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3plysqbfv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ldbofcpx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ayoznjrh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hduggzdp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kzrdaqxp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhceyvzs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3asmpjcwv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cjluaixy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wgymltqc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jkaywpyj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3sjqgxzih.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jgxunyxb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fjzqsksf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xexuoadd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fenfnmcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pioulsfc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dbkcxinz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrknitqi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rlfdvanc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lhbxhiba.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hpmhqzvf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tiqyvmvj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hbjzqmhq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nphmxyqe.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wbobaeea.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3gdepsxih.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vrxmdjrr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nkdkfozw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvdrjdbd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kopngwkv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3aniupvls.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zoinsbav.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hrmzpokc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wxehjhna.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3enidyien.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zmadbxiz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qmocgauj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ahmovmpp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ufmbdxkn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3prvjvzay.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lbpoevcm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3igxjkeac.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3drwddwwr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hukcqteg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gtkcrcdz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3whgzknrw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ptrsdzqd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ietlprnc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gmxvwtkb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vaevcnlm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ggzhxkuc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hyywcgpw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zdoijwgk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcohjrgn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3whbjfxpw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rwzuraqd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tbaulpel.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3eezjypdp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uqawzsoc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qkcvubul.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jphfvwbw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ctwcieur.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ozcqttqr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3adwycifr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oezsliym.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3htclbvxd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nypzayur.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sxnmxrza.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3aptvnmvo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qcrepxha.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3mtfvtmxg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tlyczwgu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fgfdrroa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3cmzhfdab.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bdaqoihl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdualtkb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jewnoykk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vzfaeuqa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qfeectwe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cucoogyh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eriaslrh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3silmdefu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3smkpbhbb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3omdkuskj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ajdrheyo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dqpswzma.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ressnjue.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3iiagykie.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3orpenqff.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vlxafhsn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uyxufeif.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcvatxif.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ltfuhxtr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jqriowgb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sccxkmvi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sdvwafrj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lamvidbu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3obifbfjj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mqzzhjll.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mfbjcyna.html


<!-- 参考信息 -->