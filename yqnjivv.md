代发 wailian999

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gwkbjjybv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gzisyisyd.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/ggmhgnqnx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gqdnwgjin.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gdeqsbvkp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gujsouxgt.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/grwmmgdej.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/ghwxlyvgz.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ghefsjcgv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfusjuybg.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gkdbphgox.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbyeyztom.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gjunapsye.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glvvzszgh.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gqeqzmnjm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gosystuxz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gfoxiamcp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqltrqzfi.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gwhsgvqvu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gkuhtbmhi.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gzlburewl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/guijeqnkd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/glmezgbql.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gtiymcfbi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gwocwemuw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gxsgjgigi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gjbpifnef.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gucbgevpa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gdpgwaryx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gcxrisdbt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/giitmcunw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwimdjdbn.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gjcdbmadu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxmsmhcxa.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gdtadwlxk.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/glzdwcwbw.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gzzoffrhc.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gdxknbpww.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/grnxgargn.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gmtqinxbr.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gcvhrbbgy.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gkpdjrerc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/ghzvcfzth.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/grpiulqww.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/ggzzgadlu.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gzzdopzab.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gxgaateiy.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gafktmhau.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gxzpgjkzi.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gqggnpnpq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gcaiwixwg.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gxyaakfgp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gxkzmcqfk.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/goabyajbe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gfilhsmqn.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/giflmnoei.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gwutduser.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gmxpopthh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gdvkpezkk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gfipqvoug.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gajatsyiz.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/guqnzahuz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gkhsiayej.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gnhevykbk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/ggtaelbvu.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gdtpjxnti.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmgsvttiw.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/goahusmsr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gqnonslqk.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gujrufeji.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gtvpgnctq.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/grhxqjwjz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gwqcmskrp.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gydmjsqzl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gpifnxdwg.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gbiakmshq.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gaqwhckyk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/ggckzzkyc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gitvbduiy.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gtogybnmw.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gwclmhrpy.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gcjkbswby.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gsruwhwyc.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gksqnjiko.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gpyplfijc.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gksmpzneb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gxkmdsgqc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gyoqvnbhj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gvkqilwqm.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/grhgijdyh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gpryeuxez.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gkyhmpjse.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/ghhldsprx.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/giszkiqya.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gglfzzpec.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/geikdrrwt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gvxrpredv.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gpmavexkd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gvexwvnng.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gafvemjgu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gwhsmuszg.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/geeeqlrli.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gozktbqau.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gcjzuugdv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gldtgnjke.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/ghxrfcglj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gouzgpkjr.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/glerszgrj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gydyklhtc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/guwnhohjv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gwnejbgsk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gbilyelop.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gtmncnigp.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gcyhhxifr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gvaykxcvx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gizuuaidf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/grusnnaro.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gifzfsbcc.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gpwyrxdfq.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gkywgtqqw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gileqvhwg.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gkrjvlnuy.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gffznxgei.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gxpmgydwn.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gqirvaxci.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gnbwfleox.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gsaxtpozr.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gkygokfws.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gmewdtieo.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gemdemdem.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gvdcjmiuh.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gthzlhnra.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gakjmezdj.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/ggtusxymy.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gafnxbbpm.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gflvkjznt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gfcohrciv.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gyzvqjfpc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grjnwhwgu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/ghkiwrrvm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/geqfxlgbh.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/ggflfyrts.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghldrgwha.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/ghbjhwmjg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gsgsszakd.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gkynpljhk.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gfaeolnif.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/glqvjclxb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gxjdbmncc.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gmgsndfts.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gydwbsvgm.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/ggqmmyvng.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gapibbiqe.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gfiirbfob.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gbxubjjwe.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/goplczvch.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gazyymrwc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gqttqhede.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gsjeflwft.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gwguwzpwy.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/guuuejjks.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gmiaqiclw.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/ghylrzifr.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gaeajoonw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/ggqaqdudb.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gxlgzhuwm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gklyhaqwq.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gcphssgcx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/giaxlixuc.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gkssqywhw.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/ggzcwwudm.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gwhbrhgez.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gxftobqib.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gqzmzndrg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gnfdvxrls.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gszkwmvsb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gxdyantbn.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gcaignbtm.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gkapktepo.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gafhizzge.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gizkgmztj.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gdyxmfkal.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/ghqihbmll.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/ghtckcqmi.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gqqvzkeer.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gbrpnibqe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gwpmotnya.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gftxspcwf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/glgypqnlf.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gjnhcwpqi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gdkeifolh.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gqwkprkhh.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/getdepxdq.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/grxfqoslt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gfxexpgzv.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gykvdujmf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gonpdobkb.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gbmdctuaq.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gzniowpwr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkfrwustq.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gaeacyixb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqysffzpj.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gepxzcalb.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gvfjviwdq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gxwbtdsmd.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/grgmcyezy.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gnveiiffm.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gszvisnji.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/glsouvfnv.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/ggdmdowmb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gyikcbrne.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/ghjiglyys.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gljpmdhbm.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gkdenggsv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gdlqdttmn.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gtbwqxfeh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gusiqtvhj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gkdzykzxm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gzwtmavwp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gipqyhhzb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gdjxwqdqi.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gymvhrxsn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gzevajlqi.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gbzdbdrja.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gxobfgccu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gbfsdwlgv.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gnfqvsdzw.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gxrndbtie.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gvfofgcbb.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gngxntebq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gsdeuetyd.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/goxnskzne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gscbmbspf.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/ghvrmfkus.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gnsdcciat.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gwywgqdhd.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gkysrwugp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/glbqsjgyp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gqtknziql.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gxufgjatl.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gaslbwkdt.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gdckuougi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gelmdittt.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/geyuwjlyy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gxrcznoxn.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gxfkzukgp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gissndifm.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/ggbnuouen.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gjwuhtdww.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gkoyhuvcn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gpusgzrqj.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gxvtfrdqn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gncgczcdb.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/ghlgmihop.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gdefeunpc.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gsooyapjg.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gfggiqkfx.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/ghnlxcrmb.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtlaexjlg.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gxffglsaw.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gqbmujkgv.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gocfexylb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/ggbzfaaic.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gqtisoxlw.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gvlpmiiud.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gozyqlmsh.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gqzvydilt.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gahjweyns.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gkacfrpuk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnneinxdo.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gtzdrghyy.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gwjskdloi.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gfzxmrylp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gsnozglan.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gxqvpkfly.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gsdxcrbwz.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gswtaylyo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ggixdvzjf.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gqlvmevob.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gekgwkdxj.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gzdlvuakm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gangmnzey.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gqqerkhbe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gaftidrug.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gpqtpbyva.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gwuwunorh.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/ggjrelcji.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghldaxjon.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gutjvslkn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gjeixpvzg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gscopdden.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gvphbmgat.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gjemorras.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gsnytjbmh.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gipbizgto.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/ghvluehok.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gejlsrump.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/geukgwhur.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gbniztzko.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gzzgwjxjv.sHtML


<!-- 参考信息 -->