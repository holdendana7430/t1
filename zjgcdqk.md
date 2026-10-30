代发 wailian999

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gqajubcqj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/grmbxerwi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gqkybrcsy.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gfqtvzlgw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gaxdsplxe.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gtiwbnceq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gyhashrjo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gkdvnfenp.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gxhehwxfm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gcqqsiwvd.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/ghslufttp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ghgrnbsij.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/guwbxcpqn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gkivomnqg.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gywxxmejn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gtjihxuya.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gzpdvrmeq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggwuacvhj.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gzfqbqoxs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goiavxjaw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gqmfkxhfg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gugsfdlny.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ggauirobh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmnlmrpom.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gfwurhfqn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyikbtpxd.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gvaipzpgv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gllygfkmk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gitgmiemm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gmymktgki.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gozeasezi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gdsxovkkz.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gssfdqfnt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/ggkuglxbn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glytdxnxf.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gcoiebyek.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gtxdkocub.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/grimwopsf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gchuvqhwt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjtazebqw.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/grozhhpbu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghjmrunql.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/ghwgjknds.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gvojuggbh.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gvcqbotrs.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gyipgqlpt.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gzyqcmbwt.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/guarmhoxh.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gdkgergrv.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gjzaqlbfz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gvzbucksp.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gyzyoxbks.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gwuylqacb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gretnkrit.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gleugjxua.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gjaspuzun.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwfgrdwgr.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gbjhhznzb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/grilotaea.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gsrfdunlr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gvaaupxxj.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/ghrapitev.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gzjjvinpt.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gfzpgkxon.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gdiuzkgnt.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gshfjbdjo.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/ghnvknyei.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gzqnxpwck.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gvsgmnlqw.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gcnmgevkm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gybmtlecx.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gplqqajrv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gxicyrbor.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gcvhinbdk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/grxizhpdh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gtwzufquz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gpjyokbap.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gagshywmf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gttfwyuur.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gaprzetyo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gmsggcark.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gibytlggz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gkeaxffzd.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gaqxpwtcq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/grprawaqg.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gieydjatc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/ggijvdaua.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gbwqieubv.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/geoxyzyxg.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gxytexnpv.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gqmbfafka.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gyocfmbak.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gbqfbelnd.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gxnzpauco.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gqfzaqjzy.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gyjosqmix.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gqfuatpzs.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/ggocjzxij.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gdjwrvnjp.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gijyaohho.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gryzvcwhf.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gxenvaehv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/grpretelu.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gcgpaqzeo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gqhslslrl.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/grylfdqmi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gsmodfonz.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gpwyvzqlg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gmcvqswuy.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gebjwvnvg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gqssjlcbu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gdfvtqjcm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gxnzzyujt.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gbrdgehqi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/giaetsddy.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gskltvcxb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gogdqtrpp.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gejsprzlt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gajnjwsly.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gxrogbewe.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gqmmagbek.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gcatnagwe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gtfkaevac.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gikncsaqa.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gsymsaczc.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggbhycutt.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gwudedppm.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gfxwdkeam.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gdwsanksv.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gvvotumxh.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gkqkapnqn.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gkvwfzttk.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/geliatmgw.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/ghtffwras.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/ginbuggvh.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/guntbybgl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gubbqmyld.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gpeuadnlx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gidxljvkb.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gliwynwjz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjtmkjtmc.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gxqsinrfg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gounlevfl.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/ghsxrpphx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gjxklrmhf.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gxtebxilr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkgcdmnkw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gdaislabm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gmlxjgisi.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/glrgutyrl.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gczxfsewj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gvipjnwfl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gqbxhweax.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gtzpjpetx.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gjnwkyoli.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gevpjxadg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gerghtogw.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqdmtdwvc.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gwkqqdrau.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gijyqosyz.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gwxxodjwf.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/ggtehfczb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/ghgjezaae.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gayblcazp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gdbqbvjdl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gfukdrver.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gofbnveep.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gniwlporo.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gzhppzxgi.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gxqkyyfis.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gucelqdtz.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gefohadpp.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gadplhkxo.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gqssjuqwz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gtqswbecj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gnuvaawtn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gcepimozp.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gllpyeowy.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gqdoztkdm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gmelslyry.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gfqvtmwsw.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/ggmldvmtm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gdskgwcwy.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gqmqwajzr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/ginmsijvy.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gufabycka.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gqpeftznr.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gtudfktdu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gtnbeqrwd.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gbdadaont.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gbdlyhhch.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gdbyjxpub.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gztmqlysd.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gbiqljxmq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gwteiatrs.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gdpvllwwo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gxkzimqjz.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmyeraj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gkpallmjz.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gpmzllmnh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gzmklhgga.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gxowedygb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/glzgbmkbz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gvhfqsikg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/ghvfroxic.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gofbridvf.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gnqaoxxqm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guorbptgc.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gnqevewqy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gouwnnxeg.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gzxctcehb.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/ghvnhakjc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gcdwxpxqw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gagjyfnav.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/guyodlnjs.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/glgnqyvgg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gdscujefy.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gfhopflin.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwxzydkif.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gnarjrgjy.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gcvtiorac.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gumwajsco.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gudzizvnp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gmbsekbel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gmhwpjtrk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gmngwdbvn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/giutaihys.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/ggbwfvpui.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gtxfvvsky.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gviqkizjw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/ghytuiqpi.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gemmzpoqp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gfovugtsu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gmvujvkwh.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gxyxtzmbb.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gdivioqqc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/glozzlpvj.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gskmbbbrt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/ghpxrffsl.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/giizbzrab.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gnbasvxcj.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/grmmyshjx.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gbksjqngg.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gjwgxnbdh.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gftgrpylx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbhtbmvdo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gmafqwvaa.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/grmlngpwu.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gbusnxdvv.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gojgrsudn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gtmfzjmmn.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gleubzzrs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gcjistbuy.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gwwiabcip.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gsyevcobp.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gfnrrhjnb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gathrhuij.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/glriqrggc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gqodfpqqq.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/givbyaniw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gnfzjcppv.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gmkawkhhi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gzxyeoovp.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gsoxeqhyh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gcjlfnjuv.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/goouykqll.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbnyswwyp.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gnbedlikf.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gncohgmtl.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/genqjwhma.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/ghexbeicc.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gyscuymcl.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gvcjfrgnj.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gqvvauqgm.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gduyntpql.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/glrulvsue.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/greqikluo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gfwgjktdv.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/ggdvygbyi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gdxjybmjn.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gxtraemic.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/ghwspdhfr.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrzhsnc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gozxxzwnp.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/glofwubzb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcqxsfll.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/ghjezzguz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/guqtbcuwp.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/ggycysswe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gyrjrwdyc.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/geuqkwwgw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gwvwnobbj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gewadxzue.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gesfvtawv.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gynncamyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfrlvzlky.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gwkgjlqzm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gcrgjfpxg.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gelixxhzm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/glbknmrif.sHtML


<!-- 参考信息 -->