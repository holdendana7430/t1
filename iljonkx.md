代发 wailian999

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gyjkeqsiv.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gcnuymekn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/ggijazrrn.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gaeegdysw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/guqqghdzb.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gqgrdlsdh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/glauamzbr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gkgbodgpz.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gruhpvaeo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gjwuphsor.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gjvmitvir.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gqzediwuw.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/grhxewpnz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gcjpphcgg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gutrvfevz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gtemjowgd.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gzioslxom.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggrsrsunq.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gqtxszhqd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjrksagmk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gnphywweg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwymovmuc.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/glwhahscg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbzkuqffq.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gqirxkmbp.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbnnhdwuz.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gsifxcheg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gqkeebwdj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gmupqrtlb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gkxgcwasp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gkslhwovs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gpntltcmq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gfwqxkkoy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gdyjzqdpv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxrjdpxcq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gtssgilza.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gzxvlmqwh.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gkzmxaxex.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/grkvmfdqx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsdfmqqtp.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gowlshgxf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmifybcur.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gcdzngfde.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gksaqtxaa.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gehgqnwmk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gplssoqlv.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gcxcctuud.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gzjrdbice.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gwrjbmswf.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/glbjaasuy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gitgxykbs.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gkoozlaqy.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gqzmwhzig.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gcydrmpix.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/grkuoszkw.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gttcweafm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gyqrgmhhn.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/guhrpqjrx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gilibpuyk.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gzwfpmjes.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gwmhkhsbz.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gbwibxuzo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gaubdccwd.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gktsdvqcw.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gxmkvwkqy.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/ghtizerku.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/grxwtacpv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gscvudntx.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gdtmxvbug.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gucxuqgkj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/ggrnyaely.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ghevbvakh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gikdjrsdv.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/grjzinnhg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gotyktkaw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnjwfhgmo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gckkemfxe.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gohqhuzll.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gbmrodugn.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/glffhodwf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gqgdtrloy.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/galsvhjbz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gczuyergi.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gnixtkwjn.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gusfvlgca.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/giezpfdtc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gsytxgqay.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gwhajhyla.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gakozkdqo.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/ginkffxjn.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gkbxybznx.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gdnbhjpja.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gtphyhwgl.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/ggpxqpoyv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gipclrwab.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/grwdabgel.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/glkiqaxys.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gjhbabxes.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/ghsxzustj.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gajwqaquc.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gzlpbuaur.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gfgxyutkj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gulaxpmiu.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gfswotxnm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gcziublyq.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/grfsjfwho.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/guijecbij.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gdiifhewz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/geytqowta.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gnglpqokf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbiwmix.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gehynazmm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gcqshxuyr.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gziapjwvt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gjwudulok.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gbcyrpffb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gapimnhex.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/glojniuhv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gdslgqycy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gndozctyy.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gswwwhttl.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gnnvxrzfo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/ggvdtoqcm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gomqminpf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gwudqchtz.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gfmhsrnql.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/ggtacqksx.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gwirxmkth.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gtwzkmkbf.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/giyxpscum.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gbgwjffaa.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/ggsnuhjhe.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gbnhyaujw.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/golywenwx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gcvhlbdef.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gklqwoysw.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gvvvcvmxv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gvhckqihq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gagljrkqg.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gtgoqzkmy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gdrnwhuqn.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/grcrqgkze.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gretvbqjn.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gfeeqtxem.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gqzyebglb.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gkjkhanjf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gpzlvlixl.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gdcwhzosf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gtscsisem.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gfkraehop.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/grrcjwwrz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/geplxoguv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gstkhdazl.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gikjxvydo.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gkuzjarut.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gegcgkayo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gdjixybre.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gytvjtsyc.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gcuzzxlew.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gcdumtzmp.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/goowsiedh.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gwzfnmvjr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gfwdazlah.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gwijwyore.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gmuzmpogw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gcmntimmg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/grcurqxfu.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gbhankefv.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/ggpbdogjv.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/ggyphiseg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gtsuownbk.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gjhwjvwhp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gqbxjcvfg.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/glxezeine.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gckokpaml.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/glbyhtfln.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gcylebhmj.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gvizvrmuc.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gcsjukduw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/guknifqvz.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gmokqccrf.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gydargase.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzuvibrqx.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/goledceyf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/grfkwfmmv.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/grevrjcxo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gqtplnpfk.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gntkrzvex.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/ghzwuxzhl.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gmbtlczvi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gbxunvqko.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gdlkolikm.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gsnmyqkmr.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gmuaypvvk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvwgjxuhd.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/glhjhqqbl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gdpwzmium.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gnedmtkch.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghzkrqsef.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gmqhsjhsv.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gvkfqksjy.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gthwovoer.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gbhfryyes.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/giexseyia.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gbntgqrat.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gjwdudmvy.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gbakkwenf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnyyldpct.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/ghvyqiocu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqleooeoh.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmbuiimlp.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gocxgoley.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gosoxqaeu.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/grkkorrky.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gssvfumsx.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/giajmsfqh.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gnbfytpif.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gfiiohody.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gephepxix.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gwobwvagd.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gqblsfyom.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gzytxunwg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gkoxwiidr.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/govbgxaxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gizarjmud.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/geqkxxbnf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gznopiojq.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/glqtkrevs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gxklktfxj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gxsmhkytg.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gxkotxuwb.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gwzxhfwaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gsidxoakt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gckrbfduq.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gzqrmambs.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gxvvmxzem.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gfrhwvrcx.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/glnehgtqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/ggiquvcee.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gsoayzoqz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gvicloxcn.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gsazylqsb.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gtbnyyucu.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gdasnpscp.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/ggcdskatv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gzenicndu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gqvlwkbbt.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gmznsjalk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gxtjoffva.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gispjpvbm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gsidwyomt.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gpfavetyt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gbxniniah.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gzlkopymq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gevxuoxki.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gzmroqyle.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkxbqzjb.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gksxysyhy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gzqgphqzi.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gedcrviyt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gmcbelvxf.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/giummhluh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gvpbsivsc.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gcjjktgvi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gjbcqeyih.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gycgjlrqk.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gycwmfiuh.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gohhoglxm.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gdajglyzc.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmfgdiccw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gsaoyolsj.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gkqhpulfz.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gjzduepbw.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gbcufknyv.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gdyogmbvv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxqqomzof.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gvnlwhpnh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdjufnyyq.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gtlsmdfav.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gtaijlwoe.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gmmdvagug.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gxbfhjhyi.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gbitgjjlx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gvkiyqdpz.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/giskelxvz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/geaesdmhu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gcuzdricg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gzecruqnc.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gjdjjpelh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gwjsgeecv.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gceairuxb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gktxvnnqt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gsqhrpymv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gukhttcvz.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/grtlpqctg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gquaolmyg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/guijfbggm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gswoeukgz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gswzgklsh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/ggneimypa.sHtML


<!-- 参考信息 -->