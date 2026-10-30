代发 wailian999

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfvnlrbv.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/giirzgeqg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/giqcnanpk.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvhzujuc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/geisdjzia.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gyevpshmp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbaqsduh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkxjygel.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxulscrr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfprsywx.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gyshlrxhx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbhvzgne.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gjotujnho.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhvyvsts.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/grhghphyg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnexaakx.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gpufiqigb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssztijjn.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqfsiiowx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqhojxlti.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gksojztnj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grzdoqgtf.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopozdbpf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvqbuyei.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gatoqbcmc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnorppufu.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/galayphdu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmbnfjtl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfzahmsd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gumuxebfo.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyqrprzf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gtypmftki.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyjllrmz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrmxtgfw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdznnalvp.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/geamtoeor.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gjumbchir.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsskbfuw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gfcnhkwqr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdkrvpdo.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiazjqqq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqqcsmrfd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gyegtrojh.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/ghshjodby.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksipahna.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gauymitap.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gqoycadbe.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnykufjuh.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gnccxklln.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/glrhucrrg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gthtwpgpi.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsuviwom.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghoczxfma.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnytlxyn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsojrrtbt.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbkptiwao.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdiimrdex.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghnnikjuv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gyhvpenim.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gujpihwau.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfouhwth.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gepslewxa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gcthnvruf.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gpunnrzbr.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/ghjrotibw.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/geaymbhrs.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gmhwoahxy.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwmckuatc.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gqwldbajt.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxflkdoxs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grvswzqly.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxjiypjmo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiqrduqp.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gsjleihww.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grnoznyoq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkphfvrz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gskhhtmtx.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxwhittje.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjqxjsdf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaqkjpdv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/givxpjubi.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gnoykvxlg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdzwwuqc.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbdcjdlf.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gieutkpfi.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkequjpxr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdwkfnyiu.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggzejyjyg.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjpgcvmw.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gliipalya.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasimxwcs.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsfyntci.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gilbgyktz.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsergiqp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbdrxhxhf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghssrknzc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajsylait.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtvlqlit.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gatdzumxy.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpbfnpmf.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkykejaov.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmsctytg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gmmscbddi.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvvankphu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghndpaslr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gothuaeiz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuahfunk.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcrcxbwu.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gevyahxqh.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkihklhs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsqviodmg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/glsqdhwab.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gmghbhjrk.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gvkfrewnl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkkrdhjq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhxreltz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsesvrlin.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gghhncyiw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdpqihdt.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwkdufnom.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkxtvfzm.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdyfyxhl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gbmgyhzea.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gbxjihnuo.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyrxyeua.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gifdzqnyf.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/guupuwvyb.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gfarijcrg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gankzomlo.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gmhxlzvwj.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/genvnpueb.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/goqktlaai.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxccbnso.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/godpssfoo.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/geyytewxb.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gxawdoxei.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gynvfjnvc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gxogglvdn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gacuogfca.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givaunmgv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvjebszyq.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gywibxaju.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtonekrnl.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gtumowfiv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpspkwfx.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaydgefj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gigchswew.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/ghhjpgpzk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbxewjmg.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpycqswo.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhprxvaf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/givrnwfsu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gwaphlrcd.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkofinhrh.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuapjhsj.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxvhccau.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhhluimh.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gkemhkhyh.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsmwujug.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnuttldy.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/glfogyxdw.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzydksemo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/ghlluaxco.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/goidlivvc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcggufma.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcrlssmr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/glcgegsnb.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/geydlrtko.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/ghfoezdhm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsrifbezb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlsrhulo.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuowhfwh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gmxfuvler.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gaprkxigt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhzjddxt.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gpttlitht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtofttcwb.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gssqzenyq.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkjznqnl.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/goblbfhxm.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gnawyscgf.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/geihofeme.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgpokibr.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gasohqurz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjaxucpb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gvfngwsoh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gceffwzvc.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gjucnwjuw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gtwjwkozc.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvjirkzs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnthvmkb.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gyykwkhle.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxvjfkik.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gssugitat.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsuiobqdv.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyzskpfbq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjsuyqsd.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/girkipthg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsnxrfwn.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ggmqwjtoh.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gskbvydlo.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/ghqaflwin.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzxaezetu.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gnnsyeeqs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkajkpabt.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gckldzwmk.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gmgcgqtxd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gglhbidhz.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gswudeeiz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtbbfqrl.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdrelmchq.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gcjdfgoer.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gghjuthfd.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqqzifzu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gtfzaeogz.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/glddsxspx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxdlnhwt.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gzugjlzqd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbunsylma.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzopyossg.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtphgcref.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnwtgpjte.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gwffgaarq.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/goszxapur.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gcljyaell.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/grlmfilmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gxrrxadzx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gnipuhokr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gxooaylgc.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gopzkeshh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxahzrxi.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gntgfzswv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gshtnmelt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gyvxpwmyv.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gvbozzcsl.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjuxrwxfd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzyhtsfo.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gyqxpyudu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gptfsonce.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhetkqcw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvueapfmb.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/guzkgmhfb.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gyhuxslmc.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gtrgibmkr.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/getnfmmbo.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gyzpioher.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gscgsyird.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwscltgym.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gtocjyhdy.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gavmrouub.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyuobqap.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gowomtkxi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmetjdqye.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwppvaqz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gslfdulit.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzjcjzyo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/geebbghfd.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gacxazycz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonwjesdi.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfekcnpum.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gvjlqgysf.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxvgthdy.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gxfsosogr.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gehwjmukc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gsqhpwoka.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gzaemotcb.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gicsuoyrg.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxyyugimu.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlrcagim.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyfnfgowh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/guvhchpiw.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoakciye.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gfarqdzea.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyvlnzmw.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwnrzuhv.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghojjvxkk.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbbazkwr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagkiswq.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkenckpqx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gqeakdwxs.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gimngqrhv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gtbvuncmc.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gntphocac.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gavatghvb.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gcswsfner.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdezhrlnk.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvhsyzwg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grwnrfofe.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gcmvcghcv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gnjdpiggm.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpslwdvkb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrtxcuth.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gpuwinvhp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gzrzylogn.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gbpnihdoz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzuajmfxp.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gheohbmnb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/giodnebop.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfsqbymt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geojktjqv.sHtML


<!-- 参考信息 -->