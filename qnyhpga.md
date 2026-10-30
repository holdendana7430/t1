代发 wailian999

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbstobuuc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbdpvpaw.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfagnmmax.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpnddewt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gyccxtiyy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvnbksun.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcgmkcfo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/giagyagwr.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxphcett.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyppqbar.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gurrozuat.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvvpbduh.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gdormxtvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjcxally.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvyzakzq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gystnobht.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gmtfiqluy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gechxryyv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsozjkew.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gfxxbxzer.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gruvzhxfe.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gohkcxzed.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gxxgmyyue.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdeppcom.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/glwifaiwa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gforwxeyr.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gstgpjusg.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/golzjzcoh.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gcsalwptr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gvaulvapy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhrexxsa.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghsbmshij.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxojaadr.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfakbtubo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gjrurzbyu.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/godjdqimy.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gijgxzijj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnewjgsb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyzoqsxde.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjbnyeoo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gkovsxook.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggyedztaz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpzmzbib.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpktgclqa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gwxmfzqyc.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/geponjlfu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkiagnfj.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gmpaylliq.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/ghxrkyxkt.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixdsohsx.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbpllxeh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdqkqzye.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gabimhxcp.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glbdewsax.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfcmiceh.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvshxvys.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gngpaaple.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxfryfvr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glijsdpsd.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyyvtbpv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkiordezl.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gutjrfusa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjsrosmwi.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkhomepo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/graosexcp.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/grszfkvcm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhboqanz.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/ggmjuuagf.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyeuaupdc.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjfnfagm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/giynsustf.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcimkykpf.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gijvmwjju.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvzkpqyr.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfzfzscjk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxcaxcsw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknbrlasl.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpmjabrx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggczwbbse.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gdptxxizt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gepvleetj.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsaeqnmsq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdikaouq.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbffcwdlf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/ghkxqfcpj.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ggolptkcw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtqxtgnv.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcuqgmdc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsejrpych.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvwlddcp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuyubtso.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjsnosnoz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gueqmlfsq.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gahsnkxwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnxflmdt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgqvatld.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gshlvwwbk.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gseivsiwt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gccrktxzz.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgdomckt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gosdhzhfx.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhfpzpzl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhexitaq.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/goxzzdfoi.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gysthrxtg.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdwrbenf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnsuxvxm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtxtiqbn.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gnhegicfa.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkahgemyv.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/ghdxfkjvf.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gimvoyync.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gqltnixrf.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsqxugpt.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gelpyoepi.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giofvxtdz.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gijezymjo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaahsyiac.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqxnyxof.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwoldnym.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/ghnryttyt.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gzbzhkcqp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdyqkzlv.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnoewkan.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gifwgwrdj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcesfhaer.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnsdaawvq.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpcfwyyuv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/ggaaiuppl.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsovfxhd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtxrbvvab.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/ghzllebmu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqfmeuea.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gluwrgbzt.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gugelkxmq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfyaqead.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gsjimzquh.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/glhdjzzxe.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gaybssfhp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjhopdrh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gblhwiacf.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuoznqif.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gciafzqwx.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/grhbzcztn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/geunsnhwm.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbudnvpj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdgsrenv.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnbwdrmm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gskulsokh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylpojuld.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gediubrka.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkipvpvdv.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gpamjeyzq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbbrwmtwu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gurkglrbh.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gkmlfhefk.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gemmefdyh.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gflwppfob.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsrlupbe.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcernmleh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/glgympwgv.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqubetqqk.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/geduogiin.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gczlendqp.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gihphbfqs.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxonctwsr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gymygbsqw.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtmqmtlk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gaabfwhgy.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmtobrtn.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gruborozj.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gmnvsifaj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkofqbfbz.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gbyyqprjy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtudoejqn.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbgnpgci.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gtnvvstly.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gzfqpnleq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/goggjumid.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqkzelowm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjlqqzju.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbirmtwsw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gkedvnwjx.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gyhoacnxq.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gephuhdsf.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbpqvpri.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/guufursnl.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/grmmzstfc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzruwdvk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxazzmlt.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/guywxfbfv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfnxrmvt.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gswmcqpnf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxmtagci.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/goetxhvpd.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyenfqms.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gslniifev.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gorgdsovz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gysdoyrbi.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqsqbddp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwsjszuf.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/goegseain.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcxbnfqj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ginooworm.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gvoantwhe.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfqggdyxb.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/golhjapxk.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhlfuiyt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnscyahkd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gryikvrdc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gcjgbmokw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/glzgnlwoe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhckjidk.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gnrpkmmay.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gadsdcdrp.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gapruprpl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstcsnqsu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpidzzjq.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzemsuxuz.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgnkrbzp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/geaajtouu.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gbucsnmyu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/glvhwwpqr.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/goyiupjst.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhpjvflt.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmrfnqvk.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyamjbsp.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gmlvlfbqf.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/goigdoaxa.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grmullyax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gucdnyqyf.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjbzunrne.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcotxvdeh.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxqnflmuf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnrodehh.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmwpakti.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gycsnwdbo.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxijrbje.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govonejuw.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuuvzbjg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyjsvfqi.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvhgdwaa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrohvkac.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gauxxqsoq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gibtdfzmm.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gsvcimoru.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gbnepdaxb.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gpljtiixj.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gzmsrntiy.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjstzoax.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gckkvybvu.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpcdprpt.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/guzotljdx.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefhojvre.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gkcvfnhza.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gayhzsgeu.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpnioxxf.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpmxoqkx.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvxaxwka.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkwryfbc.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gwjntbuvp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gethgesqq.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvfzgvhk.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaxzoqkm.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/guzjnntkn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gchcebcbr.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gcnvtmgdq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxpotftu.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gsogbmrcb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gesbovfpi.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gqpnrpqvs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gijcmesio.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gjfvaqulo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gneprzotq.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzslfsssd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaqrlxdf.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvewnqoj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gpwnkiklg.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/grwbniaah.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvkcawrf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjilbhtn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljexevoa.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guazgfoep.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gqcducuni.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfpqzbta.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxjkvbxv.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ghppvdkkj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzuxxjsaj.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gdmqtrvga.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwaayejz.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/guqdghete.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfouxrebi.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gboszytzt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnaagthwm.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdgndiaxv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grozndjhq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpctjfyc.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcdtbrvu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gttwvidmp.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/grfdbivgh.sHtML


<!-- 参考信息 -->