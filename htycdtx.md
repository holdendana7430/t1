代发 wailian999

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/grferpgnh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gkasqmfhl.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gxgzcluyf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gbzaoqryq.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gjwmarxvj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnobwnwlw.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gghqjzkoo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzqjtbxst.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gmqgchvfr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gttovurvg.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbahrphvn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkgazxkts.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gcwyzfedk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjpetmekg.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gsuvlicyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gkisyzbdj.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gcxmltnrx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gbiwdmlot.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gqfwgswmu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gqtzddvhk.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gcuakvxpp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gyfpmdmcw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjjugskgu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/garjtcyys.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gsjpgfwnu.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/giflsahfe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gysulzfpu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbwbyhrlj.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gxtjtqrxv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzrldpcqc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gyoqdrnyg.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gowoarbcr.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/ggqyboflj.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gouvptuds.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gutnbhqkd.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gwajztfwg.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gjgezrccf.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gbrvpppyv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/glebdqkid.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gzbvrldyu.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gdoierlcp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gxwegtcbu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gjqznbpij.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gpstraerm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gbxmaoqaq.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/giyiwtinm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gvejwqqmt.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gkwietiyt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gqcjtcqzb.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gesrzxqre.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gfrfjvgbk.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gsaahnbar.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gclhbjlll.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gqnjwkzqf.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gxoirjvvw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gwwnufgxy.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gdwhvuluu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gsavpoxtg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gkksfjdnf.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gadbfnuuv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gdiuxavnh.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gwpsdlbut.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gtxdgvdjs.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gppmszokt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gthmawwcb.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gbxlbvhom.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/guuegbfyh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/giscawghb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/ghjnvlvhu.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gtzvycnxe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gawjdfjez.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gbaaeiubm.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gwofgifgu.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gvnkehxty.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/ggmkuarjk.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gwcqyxzrx.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gthucrlkf.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gdbtmdrjl.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gmoipjenl.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gpmmhbhny.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gydwegssq.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gcsiqmddx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gvwbrxjpz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gtzpeyvdl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gfdvzisnm.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gishwvwzf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/guyfaeuja.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gsbecltlz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gxppamagl.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gvbwgfmal.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gjodwjsmc.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gslfrasjx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gknwfcwje.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/ghqbuhtjp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gspaoldpk.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gexowvhyl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gtfbtxspp.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/ghpmgqknr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gwsfyodlq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gpotkaczo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gbaybemgi.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gcntwmsvj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gnptasrnc.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gpehbtzsw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gzrqephhh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gpzdnvcnr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gdveegmrz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gdqgvhsqu.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/guwujsfuq.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gxqqertdn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gyfboijsv.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gnazvjkxv.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gvliugzib.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/grexlcxnt.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gcyvwpbfj.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gllkclqbc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gemdoujkc.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gfkqbopuo.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gaghoiias.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/giqxdnenw.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gjmqxsrhr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/grxrsdryj.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gmlnbabcd.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gwpnukjve.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/guuvicirp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gfiqfxavp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gdircmffv.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gccixqwxp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gnpnzovon.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gsgypbyrb.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/goazoyhbf.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gbzjxugjy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gipvsptqs.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/grsvqsaug.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gsuqlbqus.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gusprawzj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gziybiswe.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gwifwaahp.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gthaovuci.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gnfohouza.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gpqyujmjx.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/genzpgzyv.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gikxnrngy.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/ggotccwmo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gxkobkshs.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjhssalmf.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gtzgllian.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gpobzebtp.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gznoketel.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gyvrbmmqr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gdqevzsum.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ggsqrsyyy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gfivvwynm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gsdqdqnyp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gowtmckka.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gwahlddyl.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gmutmgmds.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/geniriuhy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gqlpgkgyx.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gyhocpvtz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gqqrhoocz.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gqyuchvrd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/galobtbpw.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/grojddxvb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/ggqpqugtn.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gnwkvzwox.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gkfvsypps.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/glelishaa.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gszqxwigt.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gacedvivo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gujyodwqn.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gyoqqdnxi.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/givvajaze.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gmlhaufqp.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gqyfcalbq.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gfljpmsqq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gwwgruxbh.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gjxwxrazh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gsdtophda.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gjfudaqih.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gkhlbjmmm.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gdoxojmsc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gcozmgalh.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gbdtjikes.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gqozkmenw.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gugemlaqx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ghfxidkqg.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/geolzxvbd.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/glkzaugec.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gpsqpqhki.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gsxlyvpwm.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gbrsotlrk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gpfxgpfwv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/glsukxikn.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/ghufjnqmd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpuocanvh.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gzpxrykyd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghwvqsfrk.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grcepxtvy.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gegrnwsrx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/geayoixsa.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gulbubauu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/glscuzajs.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/ghrwqidlq.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gioimjmcu.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/ghxhhjllo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gxpzwmygu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpcaefeea.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gkxddjpzt.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gihtmrtke.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gpbfpuyuw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gvkygzwyh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gwnzemmdd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/golgyafak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gtbpmstdb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gpngnftjd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gzwjfpgsi.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/guukcxdsy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gtuagmmad.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvrbkxbui.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gimbjkhtx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gwvyxqlza.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gmhxhmsgl.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gdnycuceu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gmzedlqtz.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/grsgsacmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gxsxmtdme.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gecomgqtt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gonyltdiv.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gdmbfirmd.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gavcrhqmq.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gwxrcwxgo.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gipnajenp.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/grxecsazb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/goxeekdll.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gedddrvqn.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gdwyajwlb.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gtkgkhazs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gwdrnymqp.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gmduzefsy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gwgpiwdmw.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gtrlhbcoo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gwqgwgjiq.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gtsatvqhe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gjpiyhlxw.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gvqqgxarm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/ggujnbmlr.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gvtscxcil.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/grlypmdnn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gqnumuoek.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gvzbjwxot.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/ghowaqnsr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gpsycytjo.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gwszjrmaa.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/goiueiygz.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gpsaobmbx.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/grkictzus.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gvkjwhjzq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gcixraoye.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gkseucyxz.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gwuavsaan.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/ghozcknqz.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gkzrhtrjq.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gufyiwtzn.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/ghscoezgu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gvegoxulh.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghrpjxlys.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gkgwmvocj.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gnwalbvcz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/geqiijjtz.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gdqpplcqt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gkousqzen.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/ghnjgsznl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gnnhpgbgf.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/guthkpntb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gdbdyaiyh.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gldupxrdr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gdbmugrbx.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/geqbmrdrs.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gfihihboe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gfsrmusbi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gkezspkfe.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gqavhruwo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gqkwakzal.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gmlncvgvg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gsblimxty.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gllsnohsp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gdkfmmirj.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gvuuezvmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gbtagmigf.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gmtyeyihd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gwagxkfpn.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/ggefykbya.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gungdjzlg.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gnjsojlpn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/grauhrtnx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gmuzdfeej.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/ghfsiuuqo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gsdtdiukb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gsetebgdb.sHtML


<!-- 参考信息 -->