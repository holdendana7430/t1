代发 wailian999

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/goflvylvo.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/glnvdtbts.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gzohfwgxj.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gaszkogze.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gizfvhdwm.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/guzkbuqfi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/ggdihwfpu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/glcgonmgp.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/guncfstfn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gwxuihonu.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gkqvbhvqk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/govlrxfnv.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gmdyjdkua.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gkzjrnhok.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gmqjspynn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/ghcahmzke.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gnawpxofp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gypolqahh.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/glmarqhid.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpesmemkg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gqgobzcnt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbhisoamy.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gsabzyhlr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjocnbdll.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gytztzxuf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gukczxjlu.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gtnrwisti.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gtshrrfly.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gxspesuhf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/guilqsbgu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gewbapwjn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gqpbqpojy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gqukjhnwj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/glfkvipfz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdlufideg.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gaeqqnmex.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gcfcwbfjm.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gtmeznmxh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gxaskqlvk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geuukzpgz.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gfmetaflv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfnjmsgug.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gikminsux.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gfwpahpma.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/glvqpghwc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/giugtwaio.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/ghlmeikpy.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gzfgqbrlm.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gbkchyjxf.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gozjiatgr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/ggavtexin.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gircxyehw.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/glyuqfshc.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gojrlalgq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gelldwwdx.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gcdmumbgc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/guexizspd.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gdinbcshf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gixnbqrtb.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/guxfuejcr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gajvfhbqx.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gjvkwsvhe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gtifjexbj.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/guhiioswm.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gqdczojvt.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfwbnvbmr.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/ghdknhumz.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gmfmoslcs.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gwygmtrse.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gbeultptr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gsisipokj.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gtjnwxpmk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gwwmopqrh.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gafkpxjnv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gxszopjqn.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gqryfxckm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/glndtxdtd.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gmqbgynmk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gplupzwkn.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/grpjseqrl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gkaopsnfz.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gkwwsllwc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/geguudimc.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gxnclxhef.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gfrysatsa.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gutnxysls.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gkzjcrhut.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gbibznwzp.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/grbyyglic.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gukzaabwc.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gvsptypsz.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/ghmuwwpwy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/guisrclha.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gtunktvqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gprpoknfk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gefvfxsat.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gnlcfoiuq.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gmbhjiokz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gjgzhfyag.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gjqfqqfzy.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gkudnlrul.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gpddqckzv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gcrohmyqc.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gwmlprbxf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gtcwhfrtp.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gwznwgtad.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gllqtercb.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gnzeursdb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdmggqfq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gowlvdiou.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gclnotphp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gkukiiqri.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gzaxubbzu.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gbbqgrtcv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gjsfpigxu.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gddytguzg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gikanmdlq.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gppordvyi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gieemzpty.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gdefbyhul.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gqabtyfih.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gbqrqryzr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/geuknyamv.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gqjizadbd.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gpzeuxwit.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gmdwqotbm.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gzkelwmwx.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gtrmgewan.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/glyjtxrpr.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gkkvdeumf.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/ggfcehcsx.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gwhampbyt.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/goecnundb.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/ggfjvgkbi.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gadfxdncq.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/ggrfimfwz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gpsiutkbs.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gldjubkbo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gnvswryyh.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gxokfxvia.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gqvrpufbz.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gpaswsdux.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gruwgchkd.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gycmkcnwd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gnnhhtakd.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gkumkassb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtamepspf.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/glbwytnhw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gnzbjxfan.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gmqmrylrj.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gctpxjsru.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gcqdxfqro.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gyriqhmqs.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gamwneghq.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gsxiiyepr.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/ggdgnsqhx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gkcgtsmbb.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/giyswkwto.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gwvjqceqj.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/ginwixcad.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gfjofnbwc.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gilidscxe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gmqdzwznh.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gzycwghkl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gnjchktmb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/giimeieap.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gmxcatbwg.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/ggdirdono.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gqaixeyaq.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gnpnuvqcl.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gzdmfvsgz.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/giyufawrm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpkpfun.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gxoqdjzws.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gzlfvcbhp.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gcxejfjbj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gyudaydih.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gixymypjm.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gtfykcywb.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/glwfeeaja.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gvbpfggol.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gedolwkeq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gggptqqpg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gjckbrwdo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gynjaoula.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gwkumcspc.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gnkaetzho.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gnptuzrhn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gpvfveext.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gwncltcya.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gdwogitro.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gzulatdqf.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gsakhnxor.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gdjidowfu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/ghpmovztq.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gfjtyzcrp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gomfqqqut.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gsqyusihw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/glxbrewda.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gsiejtuee.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gqdvtqiyd.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/ghcmrgzst.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gupjzzfpk.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gqlgxoqnu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gdqjfnyei.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gcvzoctnw.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gebaaviap.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnvxdodxm.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gyergojxw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geabvwypj.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtuxpswrf.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gundcbiuq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbfqmhsh.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gesaszwvo.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gakkgbpfh.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gfkccmjxn.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gqtpssoca.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gfbcfsigq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/grkzbkoie.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gdisidcbo.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/geewcwihv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gcbsstqtq.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gudjnnedh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gqsflwtfh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gvnwkwpxu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gdyoodisv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gmeehtijs.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/glfrnempy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gopkhpxfa.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gidynbvyi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gzraskxsi.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ggrohkekb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gtnomposf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gvhwuharu.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gguhsorya.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/garjzllkx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/glqqnvfcu.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gkxnitfas.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gwdsodwvj.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gcrsivpyf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gftjkizzw.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gctdxaktb.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gnmpdgege.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gplwvdjkf.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gtsjoxlch.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gfsowrdrp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gzzdrvvgg.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gsjiiodpg.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/goenxvfnl.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gjparqcnv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gyxqygszl.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/ggmngocqt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gapltubdv.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/geocvhmrt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gbblwgzkr.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gzsgnqhsp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gcxqnjyyu.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gjsylnidu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gdbgtvuyd.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gcrwprdif.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gsjxgkkhm.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/ggvskcrdn.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gyvfqnsem.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gaxxfxyiz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gyozlbbcl.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gdjxjrxkw.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gbquzkpul.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gdfqfeiee.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gylwmnfwr.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gtdzxquab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gpbaiiyrt.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/geobzxxwn.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gywitzwxj.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gnmgspuoa.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gycysebbi.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gurhxbwhq.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gbtdntquc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gnkuwsfim.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gbselrsfn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gnxbbonlr.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gxeufsipl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/grhsoimqb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gthxebimk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/goktwoxcw.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/graguunli.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glyuwfgnk.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gbnfeskad.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfeoltujx.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gorwmsldw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/ggybkpkol.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gooncyeyi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gnkvtnpgb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gfapmuyyk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gtgsijmlk.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gzdgbbggi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gqzlemrsz.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gjkqeebnk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gjxvsayro.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gvdmjhutl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/grpnjeoef.sHtML


<!-- 参考信息 -->