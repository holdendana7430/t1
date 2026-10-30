代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gmncslfzm.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlthwjob.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkglxuox.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gukaiwzrx.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/guvphrthb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/ggjdgkaoq.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfusixqwr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgagxwff.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/goekimmfe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gegzfbdxo.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gomantnol.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/ghnjlebvw.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gcyjvhipn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gijlnmotw.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuyrsdsn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gemlsxufr.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gaqibplgu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gefphrani.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghstyjosk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gefecjdza.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkvtlkqt.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guefuaacp.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gsukhjure.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkkcffzf.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gprjflfjk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquyubgny.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkvdnrsz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/ggelkhkpy.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgnwifrg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/guwmqmfot.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkstfysw.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gknwzkala.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafgungzk.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfufmbrh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkmnzqug.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gascxrvkx.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gappulcwa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnrrfcnn.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/grvlabwnf.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbqgerxi.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkemrehto.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/guywrhefs.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlhjrqnf.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gblqcgcmt.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gifiwmxae.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdwujgga.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gdojuxuvq.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwigojmum.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gllyzeaqa.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaspkzrq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdojrjrd.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdyjmtsca.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gprergijj.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gkydswmue.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/goqhyzmoq.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfyajxumf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiinuqwk.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoyxyjtj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gumcimtpv.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwgsaoeg.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gsdpsufqy.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpzxqoti.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gifshvytd.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gczxerivh.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gzkbokkeb.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gomakdknt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcxwihxv.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxqlcqqv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcmmaifld.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gigyxawyu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guskzjvcy.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiqobotj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gooqhrzmt.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzdxxqwn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/geywajbjy.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/ghyokfqoa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gttgaokjq.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gailspeny.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqwqycsb.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibuwneed.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbwizcrue.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gugngvggu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfeykhfhs.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gidngodfs.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjmbxqpxq.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gimvgqhvk.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtcbjdtdh.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdxqsfnbm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjmrngbwf.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrfmftdi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkezosek.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gmdrcoxwy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggmwwmipw.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhoxjxnu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/golhitskl.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/godpbdfye.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqfqhriw.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/guqbtghzz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gvfcnuymq.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdoeezxgs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gehhhhzct.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyscqbqah.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gryrihovs.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdhpsjyo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gznlvrjal.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkymxmko.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdscyjltt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunybsnum.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gbbzfrfvf.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gwbxibhnt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbfcjenj.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gjjxljqky.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/guafvjnhp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxgeezhu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsoaqylc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkybzkka.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfjnbncf.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaeduunx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gkfwvijhl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gxuaxhpwm.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gwzgdszas.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwhepeqj.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdsxucgxn.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gdfrwgfnu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gfpycsmfa.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gtshcihub.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gerqqcxfo.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzxopmnng.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqulxfdat.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvzfmhlyy.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdjcuwrec.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gmpqdrnpr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrfrztgl.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gvxawpclq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gldirnvsv.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfdxsvgqm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glfgpwxbg.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gpcfbbdwj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfimhsyij.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjyceblk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gsgzyglfz.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gjtnmpxrb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfiwnetpa.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ggshfynnb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwirbhqlj.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/glrzrrhsi.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gojrpbvvd.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gquzpqusb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxwhypp.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotvtqfpj.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpcrwrgb.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/ggtmvnzlv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gsfngycnp.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzhijpfo.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gsencfdyq.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gsphlmkdr.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwjmwdsm.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuretfak.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauglputo.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gjelxfxcn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gkklmrhtm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gymwcrxcv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gamyihmii.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/ggumaspqt.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gwfkzzyhz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhtrttox.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gujqeeuoa.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gwnlwsskb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gawvtlvan.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gbgupepfz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gemyndlxm.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqerzgrz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/giwiakevc.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxckcplu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmabpcgv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacqvouxz.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gdwmkfaxq.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gcujkavap.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziwkrzdh.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtjlhzro.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhxbirxa.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gajgxieyj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gbsisphkh.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjateylaj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqvhhjkk.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gppkvgngl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guoncgwfz.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gixoweyht.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsdfytel.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gqgxdgdrp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnlyndlv.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gegsmkoff.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gofqqgcpj.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdvreonur.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdikpfpec.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhlhfvys.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwiziivt.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnnwjmlf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcijrsnpp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqajnzum.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmadxqpdr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gzorgzurd.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gyodzutoj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhofjyxg.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/guttwdzbj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gaixkwfyt.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshljiujw.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoyheuyj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gipiurrzo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ginnjrizc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goowvzfoc.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gahrcslds.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijatcnwp.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gnycnaihx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gqlhsdexo.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gylfuuncb.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gljlaelej.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gclcohito.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/godtlbdye.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gptbafmtg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gdfdwkkec.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqdservx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtagwzswo.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gbjbcfumu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gofsaibol.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gszbzgbpx.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxtnxfri.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeqembwp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbujufav.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghenjhpbr.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gikjyjbug.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqiukwscz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gvwgmbfou.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/ggofzevgq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmohozju.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqiqsolk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gzhcsrzoe.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkwifhsl.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkprjrhp.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gxfaxleop.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcejalco.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxybcxksr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gdeygmzqt.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/grqmlleaf.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsswaxsvw.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/glvussjrf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grxftdlms.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggfrscnpk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxxpcfz.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaimytud.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpekzbbh.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gaghcgkbc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/ggkobwfct.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gamspwszm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/guenazyca.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgvonygz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjhhulgb.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/guvgfgyog.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkpijfue.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgdbjtqp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidxtwveq.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gykvcomfc.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjdhagub.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/geeqoyggm.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwshjput.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuzcxtlo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/goexifgsz.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/ggesxglcl.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlkxycuw.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdvecbbw.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gpkamgawq.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbbxbwy.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmyjokbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxembopkw.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlsmrzdu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeonzoyz.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/glmrjzgxx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gouyzwffq.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gkqqrmuow.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gngkqmzda.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxtplfbi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwexxxutl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqjvowuf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/genwawutt.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gxbnmeewm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ghotqgbyk.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnufkkhbe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gdjyoasjc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpyvrscs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gqsjtsqmn.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvyzihwek.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtbffyiyv.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqcmeyldu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcwwvfcx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqocmytm.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gwqhqbswb.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjdheqsb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gueyazpkv.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gzhlbvulx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gilrkzdwo.sHtML


<!-- 参考信息 -->