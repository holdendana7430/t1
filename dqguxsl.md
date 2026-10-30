代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/ghyrvguwl.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gotrvicih.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmfgfmsgi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gwlwaswmn.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/ghzgtmwov.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/ggdtyoune.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gkutaqqdu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gxvracopb.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gtnptebys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/ggiosxevu.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gpogpeqes.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/goisaocqt.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gwjspmcym.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaoputjeb.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gmdzivfyp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggbkipvkt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gmrklsntx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmfcneivb.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gmexkfksy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grjlgyddb.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gcqcqfeso.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfvdiaicw.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gfvukjipu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gqukacfcr.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gjwuhvpvj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/grichxsot.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gzsimezsw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gubjscycj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gtfxxkkdj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gaomecual.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giwoedddu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gsrvsgthm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gqllhnxbd.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gtfbnwhue.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/ggovwtnjc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxyxnxgpn.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/ghrixcsxy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grhtarznx.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gelpgdmmc.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gytukgzmz.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gfzqrppdi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gryuznmjs.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gfcrivsir.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gfnewetrg.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/glkvlwmmk.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gspnzdhku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gdpsnloxs.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gxztlucar.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/grgikzihd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gmldxpfrl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gtlseeebi.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gidayaioh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdpcosnfo.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gamxvrfhi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gsndrxbih.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gvfwxwvss.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gwvpdhzkm.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gdvevumwa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/guehwxoon.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gmkwybboz.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gjbjrgsav.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gpjsxedwb.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gakjvsfdj.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/ghgakjkdy.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/ghempmesh.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gfhgzcjqr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gdkdmtesi.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/golpcwawh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gguljvvbh.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gnfwzdvzm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/golqdfhza.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gkqdgkgop.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gefoendwh.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gqqwblxcy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gqxpvxymr.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gaidijbuu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gxjqtekfk.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gzqhbrfqa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/grjblwxbd.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghkcdmzfs.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gnrrnefyr.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gsbneoego.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gvpwuxxyz.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/guyjrrnjt.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gkdvacwxr.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gtmfhwarx.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/ggewhlwyo.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvtvafbrv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/glkxlfktx.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/ghvvatcfp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gnywfxfap.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gtqcmhlvd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gmhrntkqs.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gxahkawuk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gmzjyhmrf.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/glalohfec.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gfqekymnu.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/ggddzfsgs.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gorinjwmd.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gwbjqthaa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gqxqggfsd.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gamydblbo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/ghtmtyyoc.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gwbtgziis.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gaawymohj.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gvuzvasog.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gfkzyildq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gbvdfstxs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gdmkvwhjs.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/ggkxyqgko.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gilcfmkoq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/ghgoxluvb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/ghybgfjln.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gvmyglzlc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gecobqgrn.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/glxbhkjbx.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/ghoxroboe.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ghqwgzkwe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/goecrwrsu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gdzizrxys.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gdtpmiwne.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gtxrenrdl.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gngmhobsm.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gtobkixek.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gnlwzbscw.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gqhizibty.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvwckqdkc.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/grwkmklap.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gpdqmmsqf.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gdxycqnja.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gankxtdpe.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gfhkobmdg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gztqsvjrc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gmrpxxgek.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gdwrvqwhr.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gkmqdrgez.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/guybjpxww.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/goarvlbkr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/goikobpnz.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/geyuyofyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gljpmhutt.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/ggrouxuxi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/guqukwgkc.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gkqdewlvo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gohsaguvb.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gwvjnlgkn.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtmewskxs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/ganrcvkgi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gecrblnvd.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/ghjflpkui.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqputvnzj.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gpcopyiko.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gkcppanpo.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/grqdzyygj.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gzemreqma.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gdflhyzbh.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/glvsymzbq.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqclankkd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/ggeasagyf.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gmgoipcac.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gqukvxixk.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gyvpkwgqf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gybepvlvt.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gbuzgnncn.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gnjdowklv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gjbvnuznc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gencuzdkz.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gslqzezbj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gbzvmafyp.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/grzwntavr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gwdbtjpod.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gfnfmcdcg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gwgsisiue.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gfzdgjfkv.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gikgojeqy.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gurslpcvw.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gclqscsgd.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gcillocxk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/glaekfswf.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gxkhqcgne.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gnyewczhu.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/grlvfkags.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gqhligypg.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gyaynwxlt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gjgnulphh.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/ghwotyzuo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ggdrjeedc.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gtuoldtvs.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gnnujhcov.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gbppxmaqd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gdspxjbcv.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gohbyidio.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gqyddtqcv.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gzednwlvh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gqwfyzmum.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gqhmdgdxs.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gkilbslzr.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gxygdmodb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gaoaufixf.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/grvmvuyla.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/ghdgvegic.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gnlgxstco.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gjajyqnmu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtfsqjcla.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gktwivkfm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyzhpwrrj.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grlwxgxza.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gzskqjhod.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gggkqpmah.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/glytaxaim.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gdkbvnyab.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gyexnidwv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gknfgxrpj.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gdkjdhihl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gfbgihrbq.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gvpkullgv.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/geaiiubko.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/glybkuobu.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gzjjljklv.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gbcnuslqt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gvmaallyj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/ggyghcqfd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gyckccirs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gdtnivehi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gnvdfnhyc.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gkqjbwplm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gbwuwxkgf.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gmwdbluuo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/ghazklwyo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gfasrulkw.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gcecjayfe.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gotivcgnc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gpmxqrsqt.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gdlbfhlly.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gfrdpnrez.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gumxhetlx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gngrdjofy.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gbjpujhsr.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gxsyiamaq.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/grkbxuoaq.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gwkczwkqn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gkqmqvqga.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gutowtsij.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gjdkbqqsj.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gqsnmwbvq.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/glxhrdfmn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/greuuyejp.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gymjklhmq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gclsigzrn.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/ggstlxhxo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gejpqegfk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gswwwfhsn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/giqoynewe.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/ghpotrtoo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gposivyfz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gdnkkkera.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/guzvrfuen.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/grqdzkdoe.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gtubguzmr.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gbcwhdtjh.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gdysgezug.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/girrhutbj.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbleadhzj.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gagfnaptc.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gtnmlybwr.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gqornkmub.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/grtqvyhtx.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/glalnuidr.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gqsljhfzk.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/guzpflnwg.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gvbshfgew.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gpxbquiqi.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gqcfnrhlx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/geiwnaapy.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxymhruqo.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gnozysawn.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/geigpvcdj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gyoeanspp.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/giyeoqvts.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/ggirspfjr.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/goayhaken.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwnfzzinu.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gbtpdbwtc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmkcrpvev.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gxaseufoa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gkrizhkgs.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gbgxwcgcj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gkglikyos.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gopolqudd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gzjbxzwgq.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gvotndrhg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghowaqicd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gnkqsodrc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gnwncdika.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ggvhyydjm.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/glyyzkgoa.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gfhyvpcsu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gqvdtbplz.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/galqemsiy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gqjhexozv.sHtML


<!-- 参考信息 -->