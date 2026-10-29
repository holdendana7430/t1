代发 wailian999

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/ghjyhyqcq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gxprnghur.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/glpkgxpng.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gvxnhkkdo.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gtfukyfgs.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gzeobfpqw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gpsfjayuv.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gtuissvsi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gfejntrdc.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gswbmkdlx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gbauwniev.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gjuuzstim.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/guwtaeabs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/golzxwktc.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gqgcjkhii.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/grmplmege.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gtwcifokn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gepbbjwyg.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gqimrjzfm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gzouxihcj.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gnvdcnmpw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpnlspyyn.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmaeitxpj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glcobqqlf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gbrcqqvyy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grygkvcoi.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/grmsjsqxf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnfjuaxub.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gbdiqccyl.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gunplxgfd.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gtlqfvvok.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gqwqqxgjk.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gqkbsmzbc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gfpatftuo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gvhjbttns.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gpyxnmfoa.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gexdeguyk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/ggznvwdey.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gykxpsjrs.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gebwlqrcd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gmeeysvzm.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gxfqaumop.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gblkwkkmh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghfxklotf.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/ggtwfipvp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gggzvtxur.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/ghggmfapo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdgrfpk.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gagajxgnu.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/goauujcqj.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/ggfthsyxu.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gyvegphrr.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/goedirobi.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gkyfgtygr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/ggckctdlb.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gzqhttohz.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gxrqlprfc.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gaaelcbtk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gvhzixlsz.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gijhctpqp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gwahltvie.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gztksjfww.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gsgxghvml.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gnjlddhwp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gczbxiocu.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gkzkensix.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gazwhgjqq.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gqbafljpc.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gummckzaa.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gaoojaraw.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gzzxmvteh.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gzbwytzyp.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/giygwyslx.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gusmsxqow.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyvrluhii.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ghaafjdsq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/glifjdfcg.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gdmhfbcye.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gdtjolgyq.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gncyfpahy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcpajlpgx.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gexzucayi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gwmoiyuqx.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gldoqhyrh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/giwtwiawe.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gmiyqcoge.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/ggbekfwuj.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/glfvnrhii.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gdgshvupz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/grxzsrkon.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/getggizao.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gapdwxezh.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/geyjaeemt.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gnpxtoyli.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gxvonjjpw.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gyechhijk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gjxlfovhb.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gqvrlidep.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gyvsazzry.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/guxiiiwub.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gcenlnsrg.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gfzhdtftj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gitlotavq.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gmsneihbx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gvvdqzybh.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gzsxkudoq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gqscvhzpw.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gmcfapstl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gnvrlkwet.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gbfteledb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gbvesmbxk.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gxbrxxmvq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gywckdvyz.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gzypkfgmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gffskiuls.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gklicagai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gwxdjlrkg.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gmhdrccud.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gdwridebw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/goxxgmrpa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gcdccosdk.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gvahnejhb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gcnrekalf.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gbbbapvdx.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gohkfcwjd.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gadmamere.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gyyqnnabp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gdkwvbzte.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gaxlrcpjs.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gyryxpovt.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/ghkctsolu.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gdqbwzuls.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gipqpdnmy.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gomvfmaks.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gwgvnjsuo.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gkwjmgbbq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gezbsocoo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gibklxyvp.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gnvdlnplo.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/ggvottouf.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gqxubnltf.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gdfhmvshj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gpxagkkpy.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gwyruqbzf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbypwkapn.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/grjbsidmm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/geikvxnua.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gnosztqzj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gggtvuepj.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gwctlnwts.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzmxkcunm.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gecpemrsi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gxgwtsink.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gumqpwvfi.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gfhwoczck.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gwddiktiu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/ghprmamki.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gdubnduqn.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gablcalmh.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/glqsmeebx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gedohjhsy.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gpjlocugq.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gmywgvxnt.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gnnrvdubt.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/guzpafvil.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/grhgsdumc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gldrcwsxu.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gerdhmsmr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gizmbgytw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gfhznmlhs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gxhrrmjdp.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/grxvwaxxw.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gvluetxhw.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gvfnuhddw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gdpgwyjwi.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gqfrtifqi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gyinjutuj.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gffmpuywo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gokosbeob.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gmwjsbppc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gudepwwyd.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwtoxkzzf.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/glwthlqps.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gtxwgssit.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gjfobxfvm.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/geqcedwcn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpuuddrfi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gogeoeizm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gmvzbqlba.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gdyhalpoh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gvtxarspj.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gyjppculp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gbvnqgcte.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gbabsikul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gpozluojq.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gokaygexj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gxtrjeobd.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/geqnnbmtl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gdrntkqur.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gbtotrleo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gwzylvahf.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/grmazhity.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gfzgdjmun.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gpuhzslef.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gkyeicgkg.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gvjqltxqe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gfcgfvwfo.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gcbgobtzb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gmmlijrth.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/ghkveigdc.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gmowvxpob.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqlztrxlv.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gchyvxfph.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwcdiloan.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gplwftsse.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gzezgxsuo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/ghbdgnhrv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gqtzvhkvw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gjikgdkdt.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gphccpuig.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gpdzcqgea.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gbkzuffsb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gtbyrzfic.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/glefrskko.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/grofoitvc.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/glaeklqlp.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gcusgfkyy.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gipainkar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gloiztvrs.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gcdglxexc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/glmvesdtp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/ggezfuihi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gyhzmarvz.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gsgebxahy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gbzjujmwc.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gvfcvdzwm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gpeqetnyk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gkwbsmwda.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/ghdkltwjd.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gctytutxc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gbicpfxbo.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/geehrqxuc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/ghjmgwfkd.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gxjenfxjl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gcknepzhi.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gepbmmtrp.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gkdqwdjhl.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gkgduecme.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gnnhhjihg.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxlhuvcat.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/grczxqzwr.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gqhumdjnd.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gmfyafffi.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gkvajtfoq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gvmctvgfn.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gvlxckxkx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gldfsmvie.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gfftvurkz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gkwhjdope.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxaoptcna.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gyyspkvjx.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gutlzybok.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gvpffgzlc.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gtviplaln.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gjjfhdqeg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gogzsonxm.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gcwiazmdd.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/geasdblti.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gadpyvdtm.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gxsijcyhd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gqarydtud.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gisyoltre.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gihzeptaf.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/ggfrxthgp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gbpknvzbn.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gmtwkircl.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/grkzzfozh.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gddzsoavp.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/glpjlmejk.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gyptnenbm.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gpkemauau.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gtdhpdqwm.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/ggcxexllf.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gsekvwrco.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gszxepish.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gzikbyyao.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gquziyrxz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbpvnxlj.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/ggbidngzm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnxjholld.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gwofbekun.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gorefemes.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gxgtpnhbz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gzevnkzlk.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gqbgpjfbb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gnzudxbqh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gjdpbjqib.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gredjmiqo.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gnbxcbygs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gckpdsaiv.sHtML


<!-- 参考信息 -->