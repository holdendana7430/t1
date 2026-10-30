代发 wailian999

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gakuzdtry.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/guphfcgfs.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gluswusxv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/ggrqtxnha.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gqroxawww.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/geylbymba.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gwucuuvjc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gkxgqgxfd.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/geawkxyso.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaywywenz.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ghxtklmvk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwziwnrst.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gcquywtfn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsjgrrojk.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gfkxkpohz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxepfugtq.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gqoehtsyw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvcnnyprv.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gfzepinwk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gtahabvuh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/ghgoakbaa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/guthwgotd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/glgsiljpv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gmynyqhbr.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gwkkdtmyy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gtfwszccz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/ghucatnbd.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gfjugrckc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/guazuaevm.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/ghqsadzdr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gbanzxqjk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkxamdzoj.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/ggufdtsqf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjftyunxu.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gnemzwjhs.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gzpkxapok.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gcykltuqb.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/ghgpxeljt.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gjycoexss.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gzkruyuhx.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gnzgsxhjr.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/ggcelaulb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gbjroawsm.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gpwecimxv.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzhwovatw.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/golniqmka.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gufsgloia.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gezkrgyce.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gnuwuxssl.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gjmntsznf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gnoczgnth.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gonnkqdno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gljtnirkw.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gupjdfaff.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gcggsqnzr.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gyrnriyxw.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gmxykdswh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gppwvtase.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gzurixlgu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gmhtldgus.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gxfpgoljn.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/ggrasnwlx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/glmktuqra.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gqndytjor.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gseipiugk.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/guopnitqp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gphvymgxm.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwqrfiusf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gclodgsek.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/ganwzamht.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gguyouqkx.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gdikcsafu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gfhyzxavs.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gccbcfred.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gnbyffhov.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqhtotewr.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gmpnwvhur.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gohyqsasw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gyylylrrl.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gnupszxry.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gnkxopgxn.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gujyvgqxj.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/ghcvheqoy.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gyeuyvcbn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gufolfjdr.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gqprbivqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gafxdbohq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gojbuldmb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gbduyhurg.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gvztewhdz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gzqbqyyhn.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gcxylsqrr.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gfgnkbfpb.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gnpqrjzuj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gkeacqrmy.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gydsbwmmq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/givizablh.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gohsvbrbn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/grrwmuhia.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/givdnhifi.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/glqyttvxb.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gmklasnsm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gfmaibwvj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gtqslfrwr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gbuiocphz.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gmlkxaway.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gbdggyiua.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gfvujbotd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gswoxvktb.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gfpdmjbyv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gcusiolou.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gpnxnzbll.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/ghfjmbltw.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gfoyoeqot.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gcjohtaqr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gzotevgmh.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gfegbzuwt.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gqfsuknbl.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/ggudwbgof.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gttwbzctm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/goxcbtbri.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gbgemfarn.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/glwrsupxj.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gwxbozgbc.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gzjvmizcx.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/ggesmewam.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gifqfgaer.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gnuakluno.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gavpdbdrz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gpeoylxjv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gwckuoazj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gbnpatpnr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxdlldxzb.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gebjsyyeo.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gavshlwpg.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gveyrezzy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gixltpxwf.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gwcfuptae.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcnokaxwa.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gjpmtnngn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gsfhtqpft.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gorkfqwes.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gklybpajq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gmosgzooy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gcbixbeek.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gduhnauzv.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gqdqopbyw.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/ghxivkpdu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gkjrfgdmf.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/golqwyxco.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gbsghuvzy.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gthkkxmne.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gclzhdchi.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/ghuhscndg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gsmnbrxcq.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gxiwijrth.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gjuzyizvu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gizdcikzx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gmoobmwta.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gxnzzagzo.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/glmrznceu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gzypytqmi.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gkkyptdee.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gzqfuzooy.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gwsqwnoxc.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gzcvlbkqz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gpeqimsoe.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gcvevmifa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/getdiddcc.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gfwbykbfw.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gxlmayequ.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gtvgddyvt.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gjjuvcfkw.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gnnamznfa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gvjgmpkus.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gvcpjuzhz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gymhhjhse.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gledvqbcu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gjfxqnapd.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gachqidht.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gimduuiiw.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gxipqjfly.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gaekncmyl.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gwrvhtcdt.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gptoybtzs.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gnkhamrjl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gdnybhmsn.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gqhctvley.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/glfsuvrkn.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/grlhigatn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gxmedwjye.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gimvhbjvl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gsuglxghr.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/grxfmxhdy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbbevpjml.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gekulanzb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gacnnxmir.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gnrhxjkel.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gkyzxmlyi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gekjnjaqa.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gveulzpbb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gohdjwufp.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gozuzbvjb.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gblxhpqbk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gbpvzvvib.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gcbaqvpxg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gndznloth.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gqkrwrjsv.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gdksxvchl.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/guhojmyod.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/grnlhchof.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/goqkhkfhe.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gjemocqal.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gewecabkt.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gbsuklghe.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gpzklymmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gvsyutvqr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gvtxmnzpr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gxlwppqiq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gilrxkljq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gyrxtkenh.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gjqnzhsjs.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gyplaecsb.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsfonuulx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/grdwowxqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gajmdssyt.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gvbwhwdpp.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gmomqlspa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gtqsbblwk.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gksmyhjum.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/galunfwoe.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gnvqjydpu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gufzdkmzo.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gwgyddpft.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gxdzywtlh.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/grjldixpe.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gxdcjeflj.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gqgnskgdf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gkcaqwkho.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gujqtrklv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gtchihbkk.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gghqbzoun.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxkpblzuo.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gfjbkjopz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gcemjwvid.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gssgepxoa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gahxfsdtu.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gvdltrjui.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gidohngtx.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gfskfufhm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gtddfdtce.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gtbxrkrww.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/ghdsdrhph.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gypljjtjs.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gkmkvmivy.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gbnjqpauc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/ghkpgiqvw.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gkvxzjmgv.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvrsmmhmt.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gxtkyrfqd.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gtchbsyzt.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gkhuibmyd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gqlfracif.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gibwscbkj.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gobeigfha.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gstaujdpy.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gnzlqosow.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmxpkbbkp.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gjywkxmka.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghjluxuqf.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gjvvmsbnr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gvicsccjw.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gdmizkogx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/ghnzbpsfe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gjbpispxp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gwgehvqtw.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/ggklttrcj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gyyvkzhnq.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gwzseffne.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gydpsmydr.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gvepnjglz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gxsogbtjl.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gpeppeplo.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gzbkhxskb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfaqismju.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gultyhpgy.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gcpjeackn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/grkatxkdf.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gpgbwwkkw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gtpurlbgk.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gkyhlipao.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gcktahswe.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gzzvvtago.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gdshpcwoq.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gjvpxjhme.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/goezaawjl.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gkmupedfm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gcbndtqsb.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gtmihalxv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gmfmhgcek.sHtML


<!-- 参考信息 -->