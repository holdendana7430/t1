代发 wailian999

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcvdgnca.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhswewgt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpsxzzmr.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpixpwxeu.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxcucyrs.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gygraotpk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gschaqjoz.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmctqors.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkppgcvn.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtalutyn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/giotfdjsg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkqyrqsp.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gggzjetsa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsacmbrm.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrhizkga.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gavcssbvg.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/grvwwdcoz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gyxbvgynj.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnyhyndi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gicqhqsxk.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gjeglphnz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gamziqmps.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwjrktzos.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gndkyuwfx.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxjoxtky.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsswddcir.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkihwvrr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcdytejpl.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gfbgasbvs.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/geqfpqmxa.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/guarchrmi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/geiiozsjt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdkbhntf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gdethyuel.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdnkjbjs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/grfyjhppr.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxofszbt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqekbspa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrcrqzkj.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/giudwldmz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmbscsim.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/geobrtybl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaimsxlmq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guqsfvpli.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gadfvqzfa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnppoewev.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gxuvhdnwk.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gjavfnbvv.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gekwrodow.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gajwsttva.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzlppjo.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjnulgats.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gxgbmjctw.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwimlhkcl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxtclvrs.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/grmierrfp.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/giencozqt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guymmtswa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gigxcsttt.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkjyhrffm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gktztykxd.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlzxkwuv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmpxvhsma.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gyltjicpx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcdfcrki.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyagjvdc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlbciimr.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gbpopqxul.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gijcjerms.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gokxrwtlu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtilwhme.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gpelzbljy.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gejqpaldi.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grshlmknk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gslrozopq.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gpkjtyvnj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwveoltzo.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gnxbgntfg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggsfvoyhm.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmolnucsz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzgfwgcck.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjkqxxjca.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrpodhya.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzppbxvsx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkgojeiol.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gopfwqjiv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwyqjxcxb.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqznilfio.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwrbufsrh.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/guuxzskfd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyhuuvfc.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnracdikm.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtzzmtbla.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlfwpmlg.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzxpdoaix.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjzjmdpxp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyirohhg.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaoznquf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhhbddul.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gtgysomxp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnbqpgwu.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnndhtgkx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gfspehkpj.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzfzvmry.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbiipmqe.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gaypyitpu.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gfoipshnd.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmvoxecc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicijvmrs.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcdycmruy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gklbkwlep.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gryifwqnf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyljryzcd.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gheriqldr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbnumjgl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gyykrsmtg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpqrqkdm.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapagicwm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/grmmqsshd.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gzixbwyab.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomdtbazg.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmoijedf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvldzdrx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdphlsfn.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwqggxki.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrzxojid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekfhogqs.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ghohqjkay.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkurcvcmp.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuhyjrzt.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuowotka.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/ggrlprwea.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/glxcxdaxe.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdgjtyrd.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkdmauexl.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkpmxrdi.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gqznnkbvk.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/ggsnialeq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxczptiud.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gduhqnqmr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gqldeapwv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnimomzi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwbvtmna.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzrzjmeyt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnghpswko.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gqtwxthhk.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gswernxva.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyboegfek.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gjpgoileh.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/glljqkbih.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxqtfzlt.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gxteixzmy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gvluzfrll.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyqakqlw.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsthehlms.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvtbnnk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gfpxsgpps.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/golnbnmsa.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjkpkbzc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsytaxge.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxmtfwrl.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfqsxtfq.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gxqjztptm.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyurqrmc.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gceypghrs.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgqmbvct.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gayfxtfzj.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyhldctf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gzkatkaai.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gonnsogna.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfprloi.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gckbsmsdw.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gkevejdtg.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfkethrh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gswwylckt.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/grkebcbjt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiquymol.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gxfzpmuum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrgyvgpq.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlluknxz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gddnleoxb.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnhmypmc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamsbwimk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gjjvvfchp.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gyscrsxem.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/grwemkpdu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbylmzzzf.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gejmoxxvq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/getprrsdo.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gecrrntlm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkgdkijs.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbtnmbxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gxnfeyhkc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgfpdzeh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqajgasvu.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtovrqnag.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gnsjlakrn.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbanuvxts.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcixbxze.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/giivjtysc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsnumohp.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbavzgpcl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxkcfytj.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gdgbopxmm.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/godhwijih.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gajmlqhxi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkorgghk.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gtkdyghtb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmghbfhu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gginlyikp.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gnkpcabfr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyxjtlrjz.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctlxgwnm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gotigeyda.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gozdpuzya.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gfvcgbwxy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdjmlbebq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gzpqidrcc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gpzussvpa.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/glhsibrxq.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gtkxmavkw.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcfslszx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/guioseqru.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gowxrcmkx.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvmvbpli.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gphetyxrs.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcinivul.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/grsjdzakd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gigmnwvju.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfxfkrji.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeevswbm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/grpdgmgir.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gfogppvda.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwicgodgc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhanjher.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gysdxsfqg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpuvmtuy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvbpdzuoe.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gufazqmwe.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gezdefwxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gackfhkli.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gfkdqovim.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/glgafunrf.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gzblyuewv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gckyqdbsk.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwwzfshkg.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyigzohb.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gnamwcsfb.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvemrdzkj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvpjrlua.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghariuhvr.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghbqwtbui.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnayrtpdj.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbshxrew.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfksddab.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gsivtdkak.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ggernjbxw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllgbgvpj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/goorazpvl.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/geynbiiya.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/guopbuizs.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gbptkkwdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnecarzao.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gbncrlkil.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkzsldii.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gbvwzvdwu.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecrrdrrv.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gjmuxgchv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gsoxtgddf.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxijqixwy.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlwzldtd.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmzsxytt.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gidipqlst.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkboinpod.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gurwpysjq.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gpmtoyrys.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ghuptoewe.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/grsglqpfw.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdybcdho.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxvnjiybc.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gszbrldaf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjdzzvamo.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnmknzmy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwjytszf.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gouwfhoer.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqcmyeulz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvohatxay.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gknlkkbda.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gbpaokvdk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzuiwglhb.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuhadslv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdtkgsan.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/guulohljp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghuhaalfz.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntpdxcjq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gkyylrcfq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfywomnhe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gshqhgmfw.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gdsvzhvtu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gugejzkjx.sHtML


<!-- 参考信息 -->