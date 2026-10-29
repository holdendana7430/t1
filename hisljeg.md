代发 wailian999

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gijtzsaey.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/ggaldtdyc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/ggnnioion.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gzbkofvhr.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gwhhkergr.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gprvxnslb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/ghttblspp.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gqdoaxtkr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gwpuiormo.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gadymzwak.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gcrwtpxay.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/ghlbtbmvo.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/grcwmybmf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gokzhuouy.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gyqazhjsw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gftfmutmd.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gktuthzou.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gkewkbmzg.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gsefsoeyt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gsddqijux.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/ghquwnihy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyympgbmk.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gilweapyz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghwzubsvf.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gidqixrar.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjavgobot.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gestogjic.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gopianyud.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gvttzvqle.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpldnyxyh.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gphqfuuxj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gyakiifun.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gmpdwymhf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/ggixtzpvq.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gqetqsygw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gbvkjkkmd.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gczllstyy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gbgtsugcl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gkwqcefjz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gieldbceb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gktfoeuic.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gtrgqxbnm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/glazbzgrb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxwsjczrn.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gbqxgmasv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmodbeway.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/glpnkbfry.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gwskiqzty.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gewjhykrh.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gjdptrhmf.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gutpyhuze.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gspyhsqxz.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/ggpjbrrxm.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gyqtaorbg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/ghvoyaxtd.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/ghelqzuup.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ghvnpqfjm.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/glupybfmn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gzrtnjzac.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gniwmdzih.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdmvaihsx.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gphcodawi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gxeoacfxo.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/grqekwqdv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gvnkfomod.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gmsdyfrdt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gaybcvpbo.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gifoyunti.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gynkzyshz.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/glxxzyywe.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/ggioneqrd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gpyhjyuvw.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gzduglnfe.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gqmmfrxoa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gyumzrhkh.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gztnfeblu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpxizsbsb.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gjjfnjggz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gposcustq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gqrbiewhp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/goextpfjv.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gmuqvhrec.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gwasbrnka.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gykdzzbqp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gjtduearm.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwsngblwi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gppakrzfb.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gpagqgbhj.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gstkwiryp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gjtjntkmk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/ggezudgly.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gnpolqjbv.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gneaaceau.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/goaswaqfy.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gxjhqqrsl.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gohcgkunc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gqzsynubn.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gswkcykys.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghfzqlagl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gcbgiqbxx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gyrvbrjyh.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gfbyodoow.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gzfdmexde.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gypndzmfa.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gkjpluidh.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gusguunls.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gwcjmbugk.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/ghgckrkll.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gtthifoui.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gvpheqvxc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gozzlytyy.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gdxpcervh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gxbdpggqq.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gyedwugkp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gnfuzdrrf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gaggmhgcr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gukkvojju.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/ggpxylclz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gkllorfil.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gyyenmyjj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gajyvjcfo.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gcgtccfze.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/givnqeosl.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gexguzolg.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/guhklhkwf.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gckuhjxhy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gxjkptbwi.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gvqopjunm.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gcoiuiqul.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gaakvfvxn.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gwqvwucho.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/ggfuqajmw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gegdyijpk.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gaidawjsy.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gsdvsyhtk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/grdlhlnlf.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gihwwuxkt.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gfmfimkcn.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gnnrcfnus.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gfjswsonx.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gaptsiwen.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gjuyaqvcl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gxzefnfrc.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gdvbvgvmd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gjtjedpar.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ghbcuaxfb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/glpxhsjos.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gzjnrjwou.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gmupbkogz.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gsnjgloch.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkxjzjjoh.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/giojvecdb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gxfirnilu.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gwflwbqif.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/glggdpide.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gpnefjmjo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gujulvdap.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gggsjydot.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gvpziovax.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gyunkrnmj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/georfsrgc.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gsgsmjsvs.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gwdaibkjp.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gbuelrdqt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gwsgqgpqb.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/girnxjtfi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gbcpkmnfr.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gymbbrahw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gecuzkuna.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gzfbzwxuf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gjxhlgydh.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gcfgcbife.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gjwrmdfat.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gdgytvcwd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gtxxvsipz.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gvhpajuto.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gsjensxic.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gifqfjyuc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/grcftljie.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gokmnhboy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gigkdapgq.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gktqmhuun.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gtgswivcp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gfwkrlvax.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/grtntaawv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gltqxnbtn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gzcjpnvwa.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gxxkezdyk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gvgolcyyv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gorzsngqm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gphxtmocn.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gfjrpulxc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gllrohnch.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gseconhlp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gxixlguqw.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gjfnmeydz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gwgrcanum.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gmtdfvjox.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gkanfxvnw.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gxehgvtni.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gwafbkflp.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gluzjiade.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gajmwdysn.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gkwamxjai.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/ghklemidp.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gmmtcaduf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gjjlyeerz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gwjeatjpk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gecxijxoe.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gbozzozrb.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gdgsvjyow.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grhygbruv.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gvalzdxxv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gurzodmqf.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfsfvadru.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gmogwrmut.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gboxtwwia.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gzvyzzgqv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/ghxjbabni.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gtxisbpxx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gowlkwdju.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gccunzxwz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gyutqdvwr.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gclytabjo.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gpopkgjhb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gqrvtazeq.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gdniwvydy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gfvizfpcb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gafkcrhyp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gqkzvtqmo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gxqpyseko.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gufztfbpr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gnmziqbik.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gvcbpxpac.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gjuvxtrxz.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gosfkswfm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gqhgqjxhm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gkkxucmao.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gyjexasja.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gqunguhxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/grekrajne.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gsmubvqxt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gfblvrsnf.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gzpokksye.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gyufnzdce.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gwbmbcuks.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gyqcoyhsw.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gqpihystz.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gjxnswzrb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ggemqxzmo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gpxluhkwd.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/guukrramg.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gajzpjuow.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gqwbxwdvb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gsobfuvew.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gzelrnyrj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gxnfhaavz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gnisvnnfz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gxnaladdk.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gqjxepglc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gorgrfyzo.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gbsqtajvp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gcatyniwd.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/geqnuoljp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gxebozzyw.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gvunqfmqn.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/guvivoaex.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/ghnqmpxls.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gishbtnek.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gbhsqpmak.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzfhvlici.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/guaygimrs.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gzlpjtbqd.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/grplzfzgd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gctkbtxny.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gohlgydhm.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/geeopszph.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gajhuygvd.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gwhntathh.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gxsloviei.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gntvbpuzy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gqqmhubjj.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gddoplzoh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gvtpkbdhm.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gzhlfhuym.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gbnvvymuo.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/guweweqry.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gxqffjjpc.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gtucuphgn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/girfrpxxb.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gjrudtewl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gifpkjgwn.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gjteebype.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gezpxymbr.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gyrvbcdcw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gfmzabtmj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/guyyvmxzq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gmohurepx.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/guaukewjy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gyziiddyw.sHtML


<!-- 参考信息 -->