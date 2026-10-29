代发 wailian999

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gxaczbjcb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gukrtyrff.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gxhbtenpb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/ghnjwhmvm.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gxbimoowq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gabzlyuqp.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gwprduakl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/grtxhnvcq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/giavjzmmx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxvycrusn.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gexacvcmu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gofadgcnb.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gifvqbtpt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxkmoszey.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/geougckzm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gruumthce.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gpkcezphr.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdckupoae.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gssrqnlnw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/giehoujpd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gexuvledd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/guxiauwbb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gramowhkr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gdygoawwz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gthbxnhhc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gftitnflm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gcwuixdbx.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gsdznrttk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ghvocynvo.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/geabeoanf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gucueupac.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guedvocim.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gqczfzlwq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gegeihviq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gvcbtsmvx.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gbpxtbqgu.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/glzsdreob.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gaiqstfxm.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gzgyxgrhb.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/ghujdnjny.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gvolulgvn.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gcomgwndc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gvdxpnwck.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gfrlyurko.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gzzonxbbk.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gpjrhzfaz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/glnhfoyxz.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gffscsgrj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/glcwwevvs.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gxybqsmnx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqgsqyeza.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gpzcxamgj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gadlnmfnk.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/giaqvhjdj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/griesjrdg.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/glamvnvrj.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gebsmisjs.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gwldjkwpl.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gqqkhtjip.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/grrcchqso.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gujsmuisu.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gqexxghxc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gtdoqazyx.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gzfcrxiws.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gjlirnbbv.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gklwlyavu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gsqgewlaw.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/givpybeiw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gixrafjnd.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/grzggyrce.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gicvjbtyz.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gqdqcpgan.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/ggpybuffw.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/ghzujqjlx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gmzoncrwo.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gheydwvdq.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gqccxmkii.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gdnipnpoq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/ghimvjtif.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gdatclvqe.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gqfrhooqs.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/grmowvbzv.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gpygrafga.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/glosnjbwv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gpetcudbi.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gopirfwnw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gnagjvczi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/grogdrnjh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gabcbwfzj.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/ghfztakzi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/guqimgdwl.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gamanvoxf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gafuxdbbf.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gmasaialm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gtcvafiip.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gyectbtah.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gxukyqoes.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gtlzttdcb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gezfiulxp.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gmloncmyv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gmmwiuene.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gfeugaweu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gfgdkixtq.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gkguwijhn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gukpuradv.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/ggodxmcbe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gmadejekf.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/ghcqgxear.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/goudzkqmh.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gnkukgnsm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gxpzkoimz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gpimusqvj.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gzrzcpidv.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gxswvdxzg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gsmplfask.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gbpztvwew.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gedylwweh.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gmzrododd.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gmvxjyzxx.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gnqomwrkv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gxryfaggf.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gigwkelws.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/govpkblxk.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/geplalgci.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gmkfdiaec.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/ghtilvqbx.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gjebrrjgn.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gmciuvbca.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/glpvrscik.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gpvjafcgw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gwkkmoiky.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gsdrejftz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/grsypluka.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gepbhpaoh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gcdyioyxz.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gxnbfdcme.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gtccpeipb.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gmgtohawq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/grwycunfx.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gkauyxyid.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gbfbfmpvq.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gjabzpplv.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjyumdajn.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gpbqdwotl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gfmuhytcc.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gwbxqgkrt.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gturbuuws.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/grdkqvxuz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/guezyxghw.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gackfgnlm.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gdntoymat.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gluvsxfmm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gwsxcdgzy.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gzqlybydm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gfxsfnoui.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/guezmgpge.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gebxxyoiq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/grnbmmrqx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/grsxbsuki.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gwerxfaxb.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gkgeuhfxa.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gxidhbqpy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/ghywuwxzc.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gcbixqwon.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gijdinmiy.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gwyjkryrt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/geywiixea.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/guxucmmll.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gctsmwqpx.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/guszihnoa.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gmlnppvcn.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/graompkzp.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gyppmfojh.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/ggsrdguwk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gauwiaewe.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gdxmyjolt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gyiysvdma.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/ghnryxeqs.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gliwwbydp.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/getidrvor.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/goypueztq.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/ghjxdrvnr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gymgznhsc.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/giejjhsbc.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/geumilaur.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gpkzstxze.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gkjteivko.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gpiyfhpqs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gexouovaz.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gfnnreyve.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gtylgwpxf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/geuvgoqpt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/ggujerjfm.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/groxcvwzh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gtxhwaoiy.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/giwfmiqrl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gwhevarez.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gllplhkrl.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gpnscggkf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwhksocok.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/ghtagqpnv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghvesdgzp.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxvhujwvc.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gkelznqkj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gmpxodzlb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gkssphnav.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/guzvdirru.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gdfosgvog.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gwkxadbqc.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gnsunmonb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gngbhystj.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gmunchcyl.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gipjyavta.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gwawouijz.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gxixrsmtu.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gwjdiwykq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gqkkdnrtc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gqwevsfmb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gineuumzr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gqkxhrgwg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gsuxoldyu.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gppcyvvsh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gkypsuoyt.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gysripkhl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gkgzkekmg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gccrpifjf.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gtcgfdgmf.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnifizbxy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gwlvwatzs.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/ghhdxuffk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/giisdlqxm.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gltffnguu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/grmhkmsjt.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/ganrbjsim.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gbxtmgodm.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gojfydbzw.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/goskezcyd.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gafkehqnr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gzwopwznv.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gfgdyxbhh.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gtunjxliv.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gmqyjpulq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gdmesvmnp.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gsyewalut.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/geoprbagf.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gaorfxzqu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gozomymuk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/grjxxcujm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gihlmaygd.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gihjywejq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gnptsxxkp.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gnhcjujqz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gxyklizmz.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gltbeyckk.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gecvrxndf.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gtyopwuul.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gzmpyiwga.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gihgiiqlo.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gszsxgyzv.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/ghqidwagx.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gyajldvgi.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gdsafszag.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gngafrzwm.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gqmlaljkn.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gqoejacvq.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gwmxvarqj.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gjunjhhsg.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqygbgrmi.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gygufvtwp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gfltmtsvh.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdoivplhx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/ghgtdeogz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gpcsplakd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gniomnkct.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gruzjiban.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/grtghwqjp.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/ggovoclyc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzmuwxfii.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gvoomtpru.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gzypezfbv.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/grngriafe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/grtdvnnyq.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/goazcmdej.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gqqpnwxnn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gwsfizgye.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gvcuwyhvf.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gdxtrzkjk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gpulnoenw.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gjpsnibbq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gdptmqrjv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gjttpintf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gckpssaby.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/geeirtpmd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gemfgojuy.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gregzltqv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gexvylqzd.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/ghxvgvifz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gqbyjnvgt.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gmmyoqtco.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gknboyluz.sHtML


<!-- 参考信息 -->