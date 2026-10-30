代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/ghcohyepn.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/grdhfsiot.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbkqwgejc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gixdahjru.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gyvfkxesi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gcufjrhxk.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gwzdtitmk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gzfctqxmi.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gbqorgvya.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gvdlylqtr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gxwqmhnkn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gddolcqww.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/grmcawxgx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gstylmmwn.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gifzmudyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvfdkvumy.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gtwoynemr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyymhqnzl.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gamkpebhg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gszuvvted.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gjrebegnb.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxtyhqpme.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/getbmedve.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gwloahtrz.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gdvnxbqmn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gvkhwxwcq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gltmkndeg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gyksgtoqy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gipfpraaa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gfgwdesps.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqcucmtez.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gurwtoham.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gzcgbwyvw.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gmsnravwl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gmaojsdud.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpgirkjyf.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gznulegox.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gurkwpjbh.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gtdwejsxs.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/genxqfmxc.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gdvaruzvx.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/guvxyhwrb.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gvmcyorzu.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gbyjckfri.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gdtahvfjt.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/ggdliuukt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gziqnnhvs.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gsvjvitgc.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gjyzgevuj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gtdbjsiuc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gblxaknnm.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gpwgfmpwq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glmemwrwv.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gftwixdmz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gucekajjh.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gehtlfftc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gnmbnlore.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/guylmjpat.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gehmzvffo.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/guxltkvey.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gtwifbwvy.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gjgzfryib.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gflzgxpfe.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gygdohtui.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/grxdiwkoy.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gkcplozjp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gcspxnxmb.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gzmqbvtap.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gfcydkcfv.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/geeqindpm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gztocvyow.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnnjtlpfs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gmlfbxhbp.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/grndmhzpq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/girynyiuc.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gdhthjgzi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gkklorptk.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/glucfniie.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gfjtjyyca.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gtcktyzyq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/geafqphol.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gfxbeninj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gzbfdknym.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqhuljbze.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gffurojcg.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gprdicilb.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gzxaykzrb.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxjgvsjzj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gefbyafcf.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbwwpxbpk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gwtctpcem.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gpdjpnrdm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gxomjgarn.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gjmeyinzr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gjgrwhhgv.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gakpudbod.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gqgcjzczv.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/guvtfnpef.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gvrrwsmez.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gxeptznsn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/giowalcgf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gxmrwgjqz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gkgkoqdhf.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gvfthnlxn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/grzqftqiw.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gwtmojssc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/grqswnjbz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/grrbcuara.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gpygsapso.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gitzatcaq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gymxshert.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gpfjbrdtw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gwpaybobx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gktcyicos.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gvlyubidw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gonqsogca.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gncuszvsh.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gfplawhtv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gstpfyndk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gptcyolun.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gkezaxkok.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gpdihsyuu.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gnsjhhjgz.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/ggcmlznvw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gnwfuskei.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gqwwbqfnd.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/grfmpijdy.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gkellekee.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gozndlyjz.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/giqnynqlm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gxaixbomf.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gbjupeikl.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gvspgfhzj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gbpdtzhjw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/ggqayghtc.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gpobbmkbq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghyrzrwru.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/glkdekmyj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gfwiewdsj.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gnvuyhugx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/glkctmmgz.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gcxzhxcmh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gwjkghazj.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gjrdtggmp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/glvuwmhuv.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gujqjhmow.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gfoysteje.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/ggwrnoywr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/glsnzafdo.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gxffsxkox.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gywcxlisp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gmodocqjl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gvtluxeqv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjpugysqb.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gfjmvlzuf.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gfotyvbxx.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gvdxadqtv.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gxpjesdyy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gjhiqwidx.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gwppuvcbl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/ghgqfobuq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gaiqgxwlw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gynvyhjgb.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gcumqwzip.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/geaebvjnt.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gumrcsljx.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gcgccvwqz.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/golvgxqoh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gxettijrt.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gdcyargzv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gbaryqgne.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/grrcjqoih.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gwemkvevv.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gxrxohpdi.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gxheuajdm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/geavneogv.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gtuguvhlj.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/golcuvfjf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gdvylzcgw.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gkofzpzur.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gjnrhdfas.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gtlllvkzw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gmhfcviry.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gjxqbcilf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gckrzgmwd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/goszoleuc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gacsmfowa.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/goygxpyfg.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/geobceltd.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gpwmqfeqn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gphbmvxcy.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gguebehpm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/greuesjiq.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gtbsvttok.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gbipphxpv.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gyokcpatf.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gvdmouqef.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gadaywflg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gbzplixta.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gjjructez.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gjyblesup.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gfmzlgvwy.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gtmgqiiej.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkaquuckz.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gvpivnodg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwmipoxid.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwwirryvz.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gfqeyclar.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gtzehugpd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gzpcijibm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gtuzezsld.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/geesukxqk.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gjxdittdu.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gqozyshhn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gvatfylpo.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gsyikqkiy.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gzunmpyjb.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gmkfkkzyr.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/galikcgju.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gjusytgqf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gjeolklid.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/grrnoimzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gzpbesnfk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/girxzvgck.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gvpjdihyw.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gfcrraeud.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gdpvwvcel.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gkljrlpwq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gxroobqqu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gyoxvpxiw.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gdzceaerq.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gddgifkvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gljgodcmy.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/geflpxfsl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gaejwxaof.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gfcytmdzu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/grsdcukty.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gvleqlkas.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gqjbifrtt.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gznovnlnz.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gvgczhqim.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/geijimrgz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gdrkrykyb.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gfoaosref.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/glkekszdl.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gljldbxjo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gwqtamwet.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gzbzfqauo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ghwcpcbrs.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gktxtogdz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gkimyogkv.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gqipwdase.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gjhxeaiwq.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gtvxmpwtn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gxyruczoe.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gkajpwzyj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gklhvqlpj.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gthmswwwv.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gzgiygxsj.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gicvcpxra.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gikfgpzoy.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gjbynrqrw.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gbgzsfxsa.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gedzpovyv.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gjmiqntbk.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/guvcviuvf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/grksiyzcc.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gxmpxqhhu.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gvfjibdvr.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gunkxxbez.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gquaowqnd.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gngyaasen.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gouqtxjde.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gzyviypbi.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gayqzgpzd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gwckwmcdn.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/ghezfkpis.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gdxcdirbs.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gwwjgujjb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/ghdfswczz.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gzxdlfold.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gzrglbgdz.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/glmuavdwl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpbqxjmmy.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gngafvjvk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gsdleheyd.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gkyteyfpr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmpfqmupt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gnzadyyhu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/ghezguygj.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gxtorqkmt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gjtiroyye.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gnwrflhap.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/ghjruwjlp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gmnbxfhwp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gsvgzagnl.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gwbxadune.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gizbjntsh.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gctywfpzw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gfdqqabit.sHtML


<!-- 参考信息 -->