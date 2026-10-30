代发 wailian999

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gxwljfkgt.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gipkvcymt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gxutrsvyu.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gcxcpbetw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/grjzsnvnl.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/grosdueid.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/giziogvyh.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gxgcqscxl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gmucaaasx.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gibnbwjey.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpcmodhwr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gsdipqyar.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gkwvjqdyv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gofxsprkj.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gbttfheov.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gytixwbff.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gfovcognk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gmnpmboid.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gfhinqnpx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gebqmlmgo.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/ghgozilcn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaemfdcgg.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gmncsvnph.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/galuhvrfu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gpgsawpjx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxglnvnsb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gxqjuwuhc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfqftadyk.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gtlwkkoyt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcefstewr.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gmlaluouf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/groprxrzu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gajvtuiuy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gcrfwxxlc.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/geagcwnwl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gyattvkxh.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gltcimnld.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gshqgvujj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/giazmavyc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gnbbezrdm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gaffdquvl.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/grmtmmtco.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gotecwfdh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glzbjggsl.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gkauegxvx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfecmvdgx.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gtlpequqv.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gqgddvmrx.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gpndatehq.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gnnfwpafq.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gyojgcofu.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ghlnjerdh.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gihitxlyh.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gbaycmmlk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gletvxzxl.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gfjtzgsdt.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gasduuosb.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/goohocypn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gyaccjfxk.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/ggtwmvqbt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gkjngghut.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gdligizqz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gsoxeerlq.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gkvptpqrk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gzmlzswmv.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gypgiiktj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gfflvmnak.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gpplfpubu.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gcawosqae.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghwxofhky.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggeemymyf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gvcglntme.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gebpdbwkm.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gjgmimrrd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gvxoorgpd.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gpkvajdkh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gvtjnxule.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gpyrglacc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gakebzzsw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gewahiljd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gjodswepd.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gwbbtnyxg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ghsrxsnuh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gvewqukjg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/giyfehofc.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/ghutgacev.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdlqkauel.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gsppuvlcj.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/glhopyiir.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gxshpnlic.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gjjjwiidv.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gsvgcguyl.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gopytgfez.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gwxaqqkae.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gauarjalz.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gemuuvdxm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/guoasgjzs.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gpuyqwcmj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gtracpsiu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gldtnwfnv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/geynjiyhy.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gxutqirch.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/glqbcdudv.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gqvntkwex.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gptdfxbbd.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gggzsjhos.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/goockomvh.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gzsiyswco.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gazfyitpc.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gcpttzcnj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gdmqevgea.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gsjzrzeij.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gtuzsdgpn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/ggixwppno.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gitludslj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gljdumols.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gnbxhfwll.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gvddhxqio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gnjxtiiqr.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gnbedwxux.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gueewepgf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/ghyvwzjyy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gnakslkeo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gicpccort.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gtklmlcsc.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gyhnkuali.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gnzphoxsv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gymzcijbd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gcyxmmcdr.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gfzsofxfp.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gtspxzxmw.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gcsjrvqch.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtltavzal.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gqeldwomm.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gldmsomhs.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gjtowcpqk.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gdkpeihnf.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gxylzflnt.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gsqebtpmc.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gvokcbufd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gevfcwnei.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gwwppeklx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gnnmlrsrc.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/ggvwrtrxy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gawrhlefi.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ggzsdudnv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gaqmundat.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gcwidqety.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gsavnlkyp.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/glubnhisa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ghfiuqbfu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gnvhirvnn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gkpkkmuzi.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/grplnilar.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdtpysykr.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gphdvtirn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gsaylkdda.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gucacjmec.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gwuadqmzc.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gsvpvkfyc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gduwzunfk.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gcriyokft.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gqtoqgkml.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/glzlgwpzo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/geqmmutpk.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gqnkwzjhu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/grgaqmivh.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gnxzrgtgp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/ghbxrilbf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gysaxikji.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gwnfieshc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gsfoywhjr.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gyugjlyzi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gjlywsmns.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gvdzhoesb.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gwogadvpj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gktacobmm.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gxktduhqt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbphtavx.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/ghqmyijsr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gmlphihwc.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gdtkmvlfj.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gngmwvvpl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/ggsdljusm.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gwvsahlwq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gnfxsixia.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkvxenvsb.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gyqsxwfks.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gzwolcajl.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gtsjltfdu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gdjvixcjz.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gjawrvarx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gblbrddpb.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gknqqzhqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gasutaqvf.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gblsyjacn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gtmoaytzs.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/grhtsracl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gnwwbnbew.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gmttmnqll.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/ggyaqqyzz.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/geyhqnhed.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gdhdisfwg.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/girqrbmnx.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gzvoeytmv.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gmvjdpumw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/glxqlkeiu.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/grpqmhlwu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gevowgnjp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/grevcdsyh.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/guxyfokpy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbmvldtiu.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gtswtpssw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcmmicisa.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gfifbuaiy.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gwefflezo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gldqtjgqx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/guoyuvjne.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gzeihgprn.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gynwopbel.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gymkkletb.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/ggpbtaerz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gntzdprdh.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gjewnrpab.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gpmaifssa.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/ghgoqxvee.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gencxkubf.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gdqiqurca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gxtoipovt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gtrbhcghn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gqjbwikuv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/glcjeckzv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gbtezmugq.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gvxhlsgdl.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gqwrfnetv.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gbphafkxw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gqsgqyysw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/ggfyraolu.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/grtxddoso.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gfemedrmt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gusitgesw.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/ggyufigjd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/giwupjyyb.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gmzvujvnn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gtxhvdzdc.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/goxicaitv.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/ghoxiksxw.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gfyclnpaj.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gigymlhaj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxzgwsade.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gymodrtwn.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gjfeaqphv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gjhbxigin.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gtthccnqc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gexwchelg.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gkrusvclh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gkyiqhpmb.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gabosaudk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gttmuabph.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gxxaqieim.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gsxxxfege.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gcmhgqgoe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gwbasntwc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvychqqem.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gemucwfgt.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gafxxgslp.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/ggecaazko.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gobqyoltv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gaeqwkbbq.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gpvkdycdn.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gghurzbbj.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gtuddmwya.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gnpsnucid.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gttmpfura.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/ggbysdyqf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gwpeaztcf.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/glysvdlqw.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gqrnrtkjg.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/grpozsyil.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/goayzmuax.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gaptywskd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwirqlqe.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/goobmwnlx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwypqji.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/grbopfhwj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/glutkrvxb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gzppjevpo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gbtgcrqqx.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gjxpxkgoa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkrthewha.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gxfrxelam.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gmgxgkkxh.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gkmadlwrj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/ggokmgttf.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gxkdnoxry.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqpynkert.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/ggndfyguf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gyzrskwus.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gzmkhmewi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gglqnhzom.sHtML


<!-- 参考信息 -->