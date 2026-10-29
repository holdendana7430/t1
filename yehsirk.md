代发 wailian999

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gbaavnlbg.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gafhlkpxo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gmlbstazo.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gaqhjmfwl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxfezdime.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gtrngevme.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gjonljfpk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gtimbvcwd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gevbvdqfa.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gotaazuox.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/geqagvuib.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gqnpbgelv.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gnviidftf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gadugnwds.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/glvcvyplp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gqcuyuxjk.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/grfyadnuv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gknyfucld.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gzzxsxhpq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gfuuxxzry.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gfmqfikxq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvdslnbpo.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gyiglcggu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwjbvbyns.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gdrvudika.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbxoszlbd.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gvfzfnlws.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdmmsvwno.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gnknqdcye.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcafycxrn.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gefrusesi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gqhwsomao.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gujbdpwvu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gtossrbyh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gzrjeetew.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gtnvuecqy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gzblzvtfy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gokyeeegc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/geoilkcky.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gvikpvpsm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/guqncszic.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gancyhmwc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gcdrhzwuq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdifcxyzx.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gnmsuwdpz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcglbyoqh.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gvzwyfguw.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gqskfsitc.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gvoxvifdy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gcpzarzwn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gvtknyntg.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gegsjpxpe.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gyoyvmkcn.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/glkizefld.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gsrbfggrp.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/grgeflyph.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gmyuvoccf.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gihreheyu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/grnjgtfkw.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gsaaexyia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gfrueepqf.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gsrstwzhf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/girdaqtsa.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gxuahteyo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gvrrxnpcq.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gnknyeywk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gnfewuckm.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gulpahflw.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gqtllefiy.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gbqwkqqat.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gkamznrgu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gymnfyisq.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gilsyeyfr.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gukwrxpmh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gimpufnrj.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gqqvvfzgf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gfbjgtlge.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gejyyiukh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gjcrswsze.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gttugkjgr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjkmgpbda.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gcpxnlrig.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gpsylsiqh.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gohckwzio.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/giplzujhq.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gsivskqms.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gzsavsslp.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gpaeletmr.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gzkfoefkg.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gmyxkbozq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gdccoromi.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gkrdtpdsx.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gzsayxbks.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gqpvgyzxy.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gpaopuxjg.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gbkccbvgi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/grfyhjflt.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gkwjhcixz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gabhvkyvi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gwokvjpti.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gmmtxhfeg.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gcwkxrqdo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gcecfmyus.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/guoefvcik.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gepjhikfn.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gpseqydjn.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/ggktbvpzo.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gtqucbwpf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gfaqovjjv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gkyvildqf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gvimeebdk.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gyoxgxnns.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gvcrkphsp.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gbgsgfkhd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/grhidixqc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gvrurbiwf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gkjezmppn.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gyzvsfxjv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gdsbpjnuf.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gupfrvilf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/ghpznejob.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gnwmdgkpl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gpnobpooz.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gwcrmpwwd.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gkeqhrmtq.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/ggztiozye.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gnlohunmn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gurynqvir.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gudmrnhzr.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gwcfafmma.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzhyins.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gybswcnef.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gqdceedze.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gjkjmrrqy.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gxrgwoewn.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gzskugsca.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/ggrfzyvqj.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gtfsuyruf.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gwbewqkwi.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gbvntqoic.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gdddcaycq.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gmlfpudcd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/glrsjlsqd.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gyohytyrj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gaikrloqj.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/goloqnbhn.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gscbtyznq.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gweafzacu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gdefnmiuu.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gpsapfcno.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtsdffryd.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/glapmlkjg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gdausvahd.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gwykszimn.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gmmkvwmiy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gchqroeeo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gtnulspkp.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gupzowsig.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gpvallgwd.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/goygazjjo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gvbzdgbjk.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gckpfxeqx.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gzpolcrza.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gdqvtntlz.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/grvbxygnd.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gjzxqkzrv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gusfdjkan.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/grbjiahqz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gqcgentdt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gvhvfdtkf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gjhmpsztx.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gyfutbepf.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gsdqqytvb.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gmnopgajw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gbrmnqqwa.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/ggmnfxigd.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gjegyzpqe.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gwmopdldd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/ghfspeuqf.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gtvhhlnti.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gxedkoljp.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gsoyylueu.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/givcrfges.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gfptsinmu.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gbnxxvxtt.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gkiqegrtn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzjvrsinb.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gvtfbfcuj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/glakubcjl.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/grafzydrh.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gdyfkyend.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdowdoudv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gvdauecdb.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gifzjysml.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gfhthnjjv.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gqyjgacaf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gtdiarets.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gewpfcdlk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gczbaawad.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gulskifsh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gsnojngzn.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gutoamlws.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gzbmbnxvh.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gklrnxobu.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gjuhnyxvu.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gicfdnesq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gstxvrhwx.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/guqrpkkll.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gjnygxeeo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gmffhspup.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gpgjabmlw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwzwtlibi.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gtdqbjmyp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcjxxafze.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/ganqvzipt.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gtspqttbt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gqvbsqcoc.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/guskeupay.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gcavsfzet.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfzwfyr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gulzqlwyf.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gpefjukkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gbupwgffc.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqsiqiqqj.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gnodyjnrj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gmmptktes.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gwlfrlqfy.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/geujopnvq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gnxxtvnjd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gjnxavcfh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/ggjvoohce.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gvyppakck.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gpuyhmbrq.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/ggwgfshyo.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gwzuibweu.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gbjucgggc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gviawiaym.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gbbbqodjt.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gjlfcxdil.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gihfgwzek.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/ghsdcvdwi.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/guiizywdw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gesscbuep.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gcrbakzqc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gnjpjddyi.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gdapcvodz.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gswnshuqb.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gkngclpkz.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gkisulnsc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gpolxferl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/godwvtdmq.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gbrbiufko.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/givdxaqcl.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/glkcsjiqn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gewxzgpxv.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gflalybxq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxmmkkwyv.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/grpkwvpuo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gmjmowozk.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/geuizszsu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gvtlwzgtc.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gegudkgoc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gruztylda.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gmepbylkw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gdirfsbfk.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/grhtawxej.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gbrukmgcc.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gfbjnmsui.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gdolnejpw.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gzrpvecgu.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gmgfnidok.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gposmyvys.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gvspbvqwd.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/ggennfppg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gvjyntfvp.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/ggyuyfkav.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gnkwgbdbh.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/ggtmeuili.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gckrjaqny.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/giuyjcagg.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gtggveoju.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gvumpuguo.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gvutvlgpx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gyxbmpgty.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gcfvaxzcu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gsadyuymj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gqczdfbgv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gjrgbmtan.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gkpxypafe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnsdrmfxh.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gzmkbviap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grpcormtm.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gaummlcsg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gttmatwdu.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gyyrqnxhb.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gkjckiobg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gkziwspxq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gcltetjcw.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gchizavmt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gvoyptzrs.sHtML


<!-- 参考信息 -->