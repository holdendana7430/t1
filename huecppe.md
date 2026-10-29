代发 wailian999

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gezhgbufh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gkmwcloph.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/ggdqfrdcq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gpjixquca.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gehbtzmni.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/ghfpqdxzb.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gelypabov.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gpqjpiiqx.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gwczivboe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpnxjegxp.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gymnkoatj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpepiosso.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gnhordcdg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdiyvvioa.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gbulejpbt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gatdjttqx.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gmjtpqyte.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrdhpwwv.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gbkkinhhs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gsadpmpuj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gwgxsnjrz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gsvpulhjx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ggrffruvd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gfsvszysl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gaouatwpp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gpfauvmwo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcppcjqod.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gvnefgvsp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/guldgehst.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gnryneqdz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/giklkqemp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnvtgaofh.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gasmncqqi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqgykncin.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gnlnxroul.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gvlwdomzi.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gjszkqrir.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gcdhacnzr.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gqrejmqtt.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gywnbrlkt.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gfqyaynzh.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gnhxqfxsg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gkxxxcael.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gqrmddxhb.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gfjqbwgps.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/golkifspy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gdndtjfme.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/grmhpgmrh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gkxbrrmlr.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gxlhdjofs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gavoccbyd.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gnossxfsm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gafvzgedv.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtwnhkhqz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gicsgkmus.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gqpobvhum.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gegrcnphb.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gotdjxguz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gltjcxygb.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/groynghua.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gyjidyyab.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gzbhmffnp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gzhqpwuip.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/glbasgscw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdxngfpqa.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/giqctmpax.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gpbyojpsy.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/grbymrtrr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsiuprlgu.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gtletlbiu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gdupnklru.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gdlzjumnf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gggershhm.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gnrvucesg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/grqyzqglt.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gktnejmmk.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gkbkllotf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gbsiyxdly.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gyvacdvuo.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gldgizcvy.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gwdgeqlyz.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/grjedriph.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gwxycuoqh.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gfqbxbddy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gxcpbmqay.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gxoortkwr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gttpxepcx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gkgbykaxa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gicuvwfeg.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gxxbpcgov.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gvuwfkgyl.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gdarrgolw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gokheegjh.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gdpexhtma.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gokigyjpi.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gingtkpxb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gylxcqtrg.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gcxegyney.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/ggqbbstur.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gpfdnvymh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gmtmvhrev.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gfrbfwboe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gntcetglx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gmlgjrtvd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/ggmwqyrbj.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gylmkqayu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gdzadpqxy.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/glwtdralx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gjbpdjkme.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gcldgocts.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gcyinngoo.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gydbbgphq.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gxjfkyizf.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gnarmzsax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/geomapprd.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gmkurukwm.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gwzvyaytm.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gnhxgewya.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gnxbuerhy.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gtsxcnfxm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gnrhfhcqw.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gzthchbxx.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gktpzapzj.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/getixtzig.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gleapkjcr.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/ggnudzjjh.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gvcetgdit.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gsxnwtisq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gyshugghs.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/grujwpfjc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gzbddsydb.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gnylxssne.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjekittpv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gbuzsepbk.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gsnvyebjx.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/giejzardp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gyvrzlzst.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gtigwqboz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gywmfwemu.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gcsvhmnak.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gkstaorao.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gzmdcsyrp.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdhjumafy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gqloclcac.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/ghkwqrmhc.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gapqdschr.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxtfribfr.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gjmrsgdwh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gvlbijjcb.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gqvwgwjhl.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/glnukmlrz.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/glizpwmtj.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gxhwvrlrf.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/giwxxspaj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gvzxblfqx.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gvvgdfbtk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gkoghocpg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/greuaqytm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gdnauncqg.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gwifppbxd.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gbfqyiwkq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gqpzwbvxu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gmgztmfff.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/glwkfypra.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gjbnszztj.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gkemtvfuo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gayeubfqa.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gkjrlpstt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gnasosohd.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/glikmrhju.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gtgtzjkyf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gqyoolmai.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/growyqwis.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gukpaxgyk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gliuxnnzr.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gtwkxptgg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gskqeifex.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gfpgfvvge.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gnsxcbfbj.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gnqebczog.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gadwjlvzi.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gcfhyvcqj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gpjktoixa.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/ggpfusxcp.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gipfxexml.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gsbmredsb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gnjevkjlk.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ghroqqnjd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gabfznktd.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gwkbjkpog.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gwuqdtmnh.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gdgypmnmw.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gabjcuewl.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gnfezqppk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gohmecjsg.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gjpjajuis.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gwaakniwb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gmscmzckq.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gctvqjokx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goqfejekw.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gkpdwitcy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzqzpzyyy.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjzmwhdgf.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gezxlyqox.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/glsdrxmxh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gfwccfzxd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gkkwugcyd.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gnkcaizdd.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gyowfjzzp.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/girqvvsyw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gnagtotjy.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/ggmuymxpx.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gqmdnmzkl.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/grmpzsvst.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/grpvomfyi.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gsphhfnew.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gvnpkkfhj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gxjguoxga.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gpgjnvzyi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gziouapbi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gqkncnqzi.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gltxvyjfn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gvzyytgxq.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gfeeihjbj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/ggggwmnww.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gsszrmozo.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gjdelsolf.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/glrhfdssj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/golebarxf.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/ggqshmutk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gidqomjxv.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gwittecxl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gmqhdsuli.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gqqtjwxor.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/grdsmiuxw.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gjgbofson.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gdkrnauht.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gihmsbbnf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtcpuqqn.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gfyigdrra.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gsrmzvpfa.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gzpwctans.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gaxwzuxyn.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gilqokvkw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxgbdmvdg.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gplakzysu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gpunnpkzw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gzrfmieij.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gflzalltb.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gtrgkklvd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/giqhgudrn.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gixxpaahy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gvczjvjxi.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gdecmnubc.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gkisfetiv.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gwiehgkox.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfrdzscc.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gmoacxweo.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gmwrqhlsa.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gndjouyuy.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/guzcogieb.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gqrmzzeyp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gplycijpw.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gipwhylvs.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gqnackmab.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gcurqhwgs.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gdkrxqkpa.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwpfwugqi.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gqtgniyut.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gvrtocoqn.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gjecxropb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/grdxnhzfq.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gnfjhbwxa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gxyxkiscz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gocawuqza.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gwxtueyqs.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gpljshuvp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glzyzksnz.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gispdbszl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gifffomqo.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gsetxadhs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gmnsofpmk.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gziaynqlm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/grjebytrg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/getggmgdb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gdocrbhzk.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gmkuabvoz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/ghdiuadsu.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gnbcznwqv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/glfaonlbk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gmukyeydy.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gqxddpdhc.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/glnagqqfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/ggmawhypc.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gkaavsiht.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gmdymyaxx.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/genvysdcv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gobrnhbai.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gattjibjt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/ggprswkkq.sHtML


<!-- 参考信息 -->