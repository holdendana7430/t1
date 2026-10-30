代发 wailian999

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gcxiopvfy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gnjeuxmsc.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gkxljiguy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gauqpuwdv.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gyzbtdffg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gidmxvyqo.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gvkvvntah.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gljtrjerw.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gebetupak.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghnbucyij.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gcwqxkqqq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gorptmxfo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gnojhkprc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/guaqxofph.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/giddhyhoe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdwkpvwks.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gsybzcene.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnojgbbgo.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/ghvosetoh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/ghpjfmafo.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gkagcwvis.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gnuhfyzov.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gdqalgrmh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gzsyxxwtj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gmvsfckin.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gfirqyrqt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/guiqwypjx.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gcwqzzyld.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gvsozwnxf.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gzbhebuyu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gsgstghmr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grrvoymml.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gxbsaliwv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbedyxnfm.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/ghenptsgx.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gpzvykcri.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gdufcyvfr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gdxnfgvrm.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gtvrzukry.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/ggmhveddr.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gnhgqicrx.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gqkshwdxc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gfadprmao.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gzwemfqec.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/grdazlxba.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gazxnhtnc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gpbxvmlje.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gvedphpqq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gpzahyxsb.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gmknshigb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdpsxgrps.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gylkiucxg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gbjxzbjyb.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/grgcjzuxq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gyyzknmpz.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/ghzpybbcn.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gnfiqkuhu.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gaaxigzkj.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gjswxonmo.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/glkjbbdld.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gmvompgyc.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gvkdidiyj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gznxfowlo.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gtmjxveyo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gszoearhq.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gbnvlgzfu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/glfwtxpue.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gthqnxkqr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/glrilhrrg.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gurzlcnwu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggtiighfj.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gceliwtur.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjyimlmdp.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gpkhndtph.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gppsgxmys.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gohyehupp.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gcvzbzimu.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gzvrhqozl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gjiljdpxl.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gvjnpnxeg.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gchkqeien.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gjwryinys.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/grzhtpfwm.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gxzmmdlpi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/ghzqlfnpt.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gjrcdagvc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gbbyyqktj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gpucoslsx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gvftzjiqi.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gjxpmipsq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/goxictzbs.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gjhdkenxg.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/geatqgkwo.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gobvjywno.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gernpcaws.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gtcmtufrm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gikwjumzf.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gsvuevyqz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/goctmjmtr.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gobgidgan.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gubzkhrrd.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gvytkqete.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gwcqrqrri.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/glourrhtg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gusdvwpsr.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gdgygosjv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gexowslpy.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gpzlobwqj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/ghdgunuaz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gzsnkcvnz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gwigbgqov.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/glxioivtz.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gcmxxwiyd.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gtwsaiqiz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/glyvgjibt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gogfnyxtn.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gfeublwix.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gxzzfjmto.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/grndnfwne.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gukgscqms.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvuqojp.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gsperkunp.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/glqimsksd.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gdqvnqprl.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gxjcnmnei.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gjajtzsoy.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gtmnvyizs.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gcqicanqk.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gldbgesbx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gqaouxcwf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ggisdcwzp.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gemvnoyto.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gfdenlwui.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/giaowofac.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gbduiztzn.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gxecpytjm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gzvlemfby.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/grmctvtmc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gxnjboqto.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gddciscjz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gsmfbobrd.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gtikyycie.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gremqheas.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gsgdtyuau.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ghbngnujs.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/glzyugpcv.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/geqxqtiki.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gzrtsgidl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/grsxcgvkx.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gzzkyugit.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gwxopywlv.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gwffncakp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gtumvozrd.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gqqtvvgwu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gqlogdzmr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfiikbglh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gmucchvvd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ggtmdldld.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gkpqnrqbj.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/ghexbxnxm.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gihagrmvl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gmzazdshd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gbjrjlvdm.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gvezfuubg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gfmtmjhzk.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gphbejouj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gzxjscrwb.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gjwtuftgg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gzoqcyhfh.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/goxgzpstg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gslesbbpp.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gawqhjicp.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gdaswrazu.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gosbyamvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/geausrtyh.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gvzmpmvij.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gkyvnowsu.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ggzfzbgqs.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/giyskjdeg.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/grpgnzrdl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gabcellmq.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gcbgaowqh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gbpgukovi.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/goiivaxwp.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gumpfsydv.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gbhbwsfwq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gyitcdsjy.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gdquwnnyd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gfwoajret.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gvfoxcmap.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gsjptnefm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gtykghuif.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gtycsxurg.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gxckzlwld.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/goljdiudj.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gjkhuugjm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gjwaussjh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gidzastas.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gxjtqbgcz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvzgzlcoq.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gekxfnuat.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbfolmbpx.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjpkobrsl.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gadozzijv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gconydpqa.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/giyekrhfg.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gxnjghbnp.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gwbvudqsw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gvgqavafs.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/glyfovozr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gbldyzcvi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/grmrcydvc.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gswdtcxho.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gijukuaku.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/grtvoxrxy.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gbnlabytm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gtvciciso.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gwwpqmwib.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gxcvnjumo.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/glwitvldw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gbuhjmuqj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gfbctoquu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gcnygqtsl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gnppzofei.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gxfmeyzpc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/grosefmvj.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gmytqdrea.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gcywqvzrc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gxhauymgm.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/glvqimrgg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gkbfuhpep.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gvckyprqd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gwpupwfil.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gnuvqddgy.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gwqkirzst.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gmzrwngaw.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gsrmysydf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gwqbhvzjk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gftuutvtb.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gtqnyroyj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/ghcflreah.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gbispsydh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gkwxxtixz.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gppljaqbg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gnalqbzmf.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/ghhmkdcnh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gkhphqtfj.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gkmfwjgpl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gincbpboe.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gfhahvyvv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/glaznvkvi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/guyhcpwql.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/ghxzckrwi.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/ggqwaqrog.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gegjjaqgk.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gfsdulrex.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/golliytkw.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gavslzmxm.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkgnybpgd.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/geqkfiexa.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gfunxmeoe.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gvhjknnpy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gslnddjvg.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gjjrphpky.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gcmgrtgup.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gqiwksfiv.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gwqycscam.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghgcdnhvm.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gaxnkfxsa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/getgsncha.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gnqtilhuf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gvedfrbqc.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gnzuldkeo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfcsubusk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gstdlizay.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gdouwmsfo.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gwgxkfqeo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnjrydcby.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gzqfsikkd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyepabhou.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gmodkujly.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gntwttzht.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gyidiezun.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gaophpfhu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gzxrtbkon.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gdpwsvurr.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/guhpjutvp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/glurksjtw.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gwyzbbnsx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gxhqumdkd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/geislgujs.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/ggnptxcrv.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/geugaskpe.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gzaqaicoe.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gkcixcala.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gsruseoya.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gbblptnit.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gizqneftx.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gewdfygxl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/ghhysquql.sHtML


<!-- 参考信息 -->