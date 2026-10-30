代发 wailian999

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilxtlqbj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/guedsmpue.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuwfhujs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvynspbqc.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejexrgdz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabgilzfw.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gssuxrkdg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gjiwpyiwq.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gltajffqy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gemuwxehg.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gaolbtiqu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gshlscmld.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmxyzkhoo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gizmpfwsd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjonazcvb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvhzuwsgb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysflxbax.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzdprykir.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gphmfvwhv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdjdmcvg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkefopuv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gfocrdjrg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmodfczab.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gjzfovuas.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwkalong.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpceobhz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbkvtubj.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gfetfwxzy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmpzmtvw.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gokyuqctd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpsnjsaq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grmvgfoow.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghheluctm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnapnccx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gisecbnud.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gjegmepfj.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gedwtfkun.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gxftvzcgs.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxjqdujx.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkzbddsla.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gkwzclbnk.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjuwetew.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcokywyhq.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gmcwkomcc.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzqfzfhnu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gltvkoonp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhskltpq.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmrflpwz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdtkzfpx.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gapwjeuaj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grabtbpya.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gebsxlwfw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghitzsonz.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gulogozwq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkpmvjgs.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonlyefjf.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gffkwglpb.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gnlirkjof.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaowquoj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gezyezuur.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmpawpfp.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvdzvsgm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlbvclma.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrervoce.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrdbsodw.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgmwuvvn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbyitzfi.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gakissnoq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gezyjihpc.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gydppijer.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcycpyas.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gxmowgdhf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/geghaijku.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhpqekfr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gogwgaqri.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjycjtbsj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbhyuctd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrcbqxtp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlvatpkp.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gturpqkka.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjffbykmj.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtyxoovs.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyedokdxr.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gercsmfdg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkegefgx.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkibgwqkq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokcsrapy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/glkvvikez.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gatlhgmbk.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbtmsvhfa.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcryrghky.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/godzpbccp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdmfinma.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonoyvqhd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlqryaip.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyyyomrhq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkiteghoc.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxuqxfib.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gcupwoubw.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfchxtjeb.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxflzgle.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvoxgscm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzspcmlfq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gzprrwbit.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gyetbxlep.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/goppztnrq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/giyunlxmn.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqbdqakz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/goqqcnyrz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gylaykguc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbojkyuq.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/guepofhhw.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvgfaskr.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gcayqticm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gopsrzdio.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gmelucyhi.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaypvrjf.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/ggsbswlii.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gsukpefrt.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ggewitfqk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gajabdvek.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdgzsebb.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geyqjxbyk.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxxbznwgj.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/giionuagm.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gifjfxnsj.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ggckidetm.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfppkoto.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gvewowred.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghphsirlg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gwburbabq.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghighaufa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbfyksse.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvtbbyrs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxebaaxeg.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdhbgesqq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gvzpltmdt.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsjdiphz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwzqnjwaf.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gkvkkltzl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gdyohnzfz.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gcklnazuj.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gppdcfhii.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/glqzottrc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghblsefnu.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghoqkrzsu.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcwuadbs.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpobtrtz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqcqykxu.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/glggqufjt.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/grmgyzvxo.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gmvlomzqx.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/guykuzqhi.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghcmqoszl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gystsofje.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdwfvwfz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gezkjviou.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmndmkwaw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaukfsyg.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsbeakqj.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/galyxotya.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdwobvmu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/garwhrjfl.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gaksxmuqd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gltdaneuu.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gzezglfae.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gswbckvix.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbjwhtvb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gvutlbknz.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/glndhwjhv.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gbeslqxgq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxplkkbwn.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcrxdmtv.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnovxulao.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwxriiqpa.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjwofhfu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqomittl.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gnsbrycig.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzclknxhx.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gjsjvfodz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gmeaccznf.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gipxbwwti.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaanksul.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gypdnwssc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyogunvy.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxywoirb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzihreetj.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwtjuluap.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtuthszw.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyaojywlt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gcptxmkql.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gtykuiqyq.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhvqwdwq.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/ggicvnyxf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guwsaynex.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gefxjzgyd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwrybmwgu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ghdsvldlr.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gstqrcpbw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbrmfoxmb.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gfteytukn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwanpdihg.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieqoxrge.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqrytlbm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgyymkwc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmheqpsyj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhwejzrj.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjefsmznp.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gosyuilyw.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gekqzlgqj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/guvrxnbxh.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxdhxtnf.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqnfwyst.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gnkymhrpm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdbyqhar.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxprxlgr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gtphwthpq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqeaqtk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffmxijes.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquefkqsk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gluzweerv.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvxhoqgo.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/geqkvvbes.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznbserpf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgekiodo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwysmtfd.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzwzpwbe.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzobnmzl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmecrwfeo.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsvqdfft.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gihuumosd.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gzlnufigf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gtfspalym.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrylbbw.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqrtppmr.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvxpgowh.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gderhtjmn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpndwatq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gxrlbzgkb.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gywonlenv.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpavqbkhu.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/grnnssffv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/guadhqrnz.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdirsukan.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gjqopmani.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gemxfvghz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gdheivypa.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gphmizizb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gohyoegmx.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gciuutzxn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gjtlglwzx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkoybstg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/grafamgmm.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmtaqruwt.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbmjgstj.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gdnvmyppw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhxvjjhf.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsanpvwgf.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzelfsak.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqtqygtso.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gxerleioc.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqticnriu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqilunvu.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/ghyjdozby.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gcplborpc.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqfvhwzu.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gpazqmrtq.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glqblzsrm.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gidbeqadm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glkwlqoun.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyofacui.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdbwpvfy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcttqvbug.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gosbkhoyr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxhopmgm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmtjwug.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gdpmtckzh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gixbmimoc.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gojcquqoq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gedyowcsm.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/ggqzuulwa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcunvbyir.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkhpctzmx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfekrjxu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/ghmqbtbar.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzszwenkr.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/givnhtrkq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gdxmineou.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gydikcawg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gomzqteeb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdfhbwkx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/govddtwbr.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvxlsmmf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhazlkww.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlwdimpf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmatfcjre.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhdodufr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbqsdgst.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwpfhfdc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbguoaqcn.sHtML


<!-- 参考信息 -->