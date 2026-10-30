代发 wailian999

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gphlsqgwb.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/ggvpzculo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gygiejxuq.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gxyimrayq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gbjvlfrwd.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gpnuczvoe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnlulwpua.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gdtoctrjm.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gsgqopjdf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gkrzyymsw.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gzwmphnqo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gxdoqmsbb.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gceiksiaz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gygbidpzb.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/glhcdjqmw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gtlitqirz.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gmjtobrlz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmvijwkdo.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gbywjdrvs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqfydbujv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/garxjxaaf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkdbecfan.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gwyrytndt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/giaeyctzg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gjdndrxhx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gfmfogwyn.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gxazhyvyg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gipjljhqn.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gmprxwxfe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gqbyggjdz.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/giouohrmr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gapvrzbil.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/ghywcqfea.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gshmywemb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/grwcowest.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gbcpyswmw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/ggctanyqb.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gjtrwddev.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gtjhldzss.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsjvmdlwb.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gqbfziiky.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcjxytqcb.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gklvuodaj.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ghsepornm.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gnwoxilni.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/glyqzkqme.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gzquzqzoj.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gnlgzwuoi.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gqlqznojn.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gxqmubbmf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gdpvqwzli.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gyoqxakkp.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/glbtntqrb.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gxgkcdfve.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gsnkmfyag.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gvdzrpyie.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gsiiqtuvg.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gokdefpgf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/galwhqpyb.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gppzpclou.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/grppozkrz.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzgvanwfe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gvmkgjodl.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gpgvvxlha.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gwhdqwtqq.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gsiqcxgsa.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghedqdycm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gukwmhqyy.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gmotucegd.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gdwijkwdv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/glnpizneq.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gsrjyhyfc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gqxzkorji.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gjwuvhvho.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gvmjybdek.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gktxnbolc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/glmfywtya.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/golulzhcm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gtshaanky.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gyxyhxtjh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gyvdkknuo.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gdqmmdege.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gvakafsen.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gpcrmprjx.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gtfrnfhrd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gtfngkpql.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gvnvxazdu.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/guifwxaoe.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/ghmivyfqh.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gcuaprbuf.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gutpkekbd.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gblwfhmiq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gorxaoqdp.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/grhavwhmu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gfvoqxxah.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gtslkwwkr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gkxeskhws.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gihnybbqi.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/guznjxeoc.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/ghrxpylka.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gfbvawzff.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gbgnfutyl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gxycbpqiw.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/guozupxeb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gtutbzlbq.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gnjzdepsn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gyimbodsg.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gtfoeogpj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gcckkxzzq.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gdwkfppyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gpkrtznrs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gukfqvche.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gubnuxing.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/giugbsaen.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/glsuqsjle.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gskwsuqyt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gdaezykzf.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gsyqybhgt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/ghejswlrk.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gkrkbugnt.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gioqadpor.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gtbfdxtyk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gglreocya.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gacwrbycs.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gykvafkgm.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gzdgfiqir.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gxuzgxdeh.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gxfxgpngk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gehvafcfs.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gcrarsrow.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gniplebve.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gfqqiuqzz.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gqmxvvjdh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/geigspgqo.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gsmwqazbz.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gnwxgqroq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gnglhvbdt.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gnboeeodn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gxnghpcbq.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gvnyusdcu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gaoswbpim.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gjcebrvkm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gjthvanfl.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gwjbrxkfh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gaqvwbhjh.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gobbsmydb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/githpxnqg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gccevxjjq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gjffvkkbl.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gwvsqzkfu.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ganxmzhyn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gftkbfopa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gwnjyzktp.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gfhxlbqfu.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gexpiqoxf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gvvppribz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gbkcsabli.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gchyahdgs.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gdyfwbnst.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gsmsyrugq.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gwsmmxqbe.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gyqmoldjt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gqpqzpgov.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gstkwgwit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gflwxwdal.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gahljhvkh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/grriupsqu.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gwpgivpmm.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/grnimhmmj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gwbiasbtv.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gshkjqpgq.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gdbjwjsnr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/ganpxeczw.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gokvbxkqe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gfjrdluld.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gvtszmkdf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gecemcift.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/ghdqklonz.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/glhnmains.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gusqtkjcs.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gpizlkypb.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gmlkqabkl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gcpjabxro.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/ggqgqjcww.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/govbscauh.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gdccujyah.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gtxduoqux.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gmlfiaaug.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gctdsqfkg.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gcoafvxdj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gdjyojifp.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gybejducs.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/glnwiedzj.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/govfnjdis.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gdlircikx.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/guqhhfshw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/ggtovzocd.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gjabwywla.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gptghfqrj.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gkgdjrymh.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gpaqarosr.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gwtpcxbfy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gpzkfiniw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gpekxuiar.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gagqlqwxa.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gantgeuqw.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gvlrhfqer.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gakblodfz.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gkbxvxnbz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghjrsnytq.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwwyekttm.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gelrhywuo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/ghurvdjfo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gyjolcikk.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gcgdnfixu.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gkgfhalau.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gfgdjnqfe.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gtlsddcrk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gqwvtramg.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gqjkyrhly.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gatrtekml.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gdsptdaqi.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gjphxslax.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gbudjnqqp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gjpatkazx.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gafeczuue.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gfujymqku.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gaxxzrcba.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gwavpjkai.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gvthezlfd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gcrkmrtvi.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gutxictug.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/giotfasgl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gdkatriob.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gotaspjdt.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/glqspugcd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gcopntfuw.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gfnahqets.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/ghsaolbed.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gogjakwmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gprwirihl.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gimvgfmui.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/ggcqfoqqi.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gcaqgcpze.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gkfromgzx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ggdltvcbt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/glckkmolk.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gtaoztpeg.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gsjoegjck.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gkbmsjnff.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gnwwanura.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gswseyhep.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/guyoebhwt.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gsnqqmqjh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/greynsmwl.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gkytnkeln.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/ggfbuouvh.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/ghxnuqvmt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gbrtngyom.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gjzjspzzr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gacqokypv.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gkozzfgfw.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gcnrmwsaj.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gimlmmgub.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/ggcaunnch.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gxhkeffea.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxnlpiztb.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gfrwikeox.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gngafbfcb.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/guwsxiohr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gwnpcdeln.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/galmphqxb.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gmbngugja.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gfeicxpzj.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gpkmramxo.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/grpzayyjo.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gpoboymrx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gbtauznze.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/ggjfrvpio.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gsozkupuv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gwswzoart.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/glzlmofhs.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gyhvlgwap.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gpwzvezyf.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gydpuykhl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ggbsonjeo.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gyugsgxtf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfqokghmr.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/ginzppadd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gafryivvo.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gzzapwgum.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/giwbvodmd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gvnmnpgwt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gsudsiigd.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gkxdiiywf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/grhknrqrn.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gwycdhhcw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gjrpqkvdp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gviewmaiq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gyiptheri.sHtML


<!-- 参考信息 -->