代发 wailian999

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrsjwwql.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhstgtno.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqoubjlx.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxzstgqc.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcyoelud.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdumvumh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gsymqcqvd.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gmmdpehno.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqajuyqnf.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/goxcyqvnb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ggzfoojub.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gxpykjukv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmhfbrqy.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/grwebfksz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuyxogzk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvxjzphs.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gofkziqkk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/ghqtqcrcp.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gvrtgkswi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhdpatpg.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/geynrtehk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqduecknx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcnvebrs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwpavziu.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaakrmoh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrtafykf.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnknhlgtq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gadunuzii.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gygyezyts.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxzpcalq.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfjlcdyj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gerfbevyb.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gdbzkkupc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvydzeacm.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gbfcfbbqt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gvjgagzyc.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gomancdad.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gpgjthujz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gekwutnkl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gbhoratlx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gmeuddgib.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpkfuloj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyehxsvi.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gonqcnkwq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gfjgigqhj.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gomgespub.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/goghjhdiq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gievcxpdy.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gflxqvaad.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbtrqqwy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grckqsstc.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gzugcxcis.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkummqxr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/glpwupzwj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfcxaebv.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkutzpmmp.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gapsvmczq.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gryfjhhdz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoyuegbb.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhkwnxmq.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdumcapux.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gnugfeupm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxmiiimtz.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggumtyrtf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvcrbbqsa.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqhmlsxa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gizilrgth.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrtfwsoh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gaawcgbew.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gggobaebx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwtflbhfg.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gzzvgqwok.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gehyftqmf.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gglunnqmq.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbqfmtcd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gkrmhindz.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrtefwvw.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzzwravzo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwvtmpva.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/glbgbjjbm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gercybzou.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gumhdiiid.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxxuqkbid.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkiobheu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbszaazgu.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/guycuedwc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gycwcjoqd.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/grucewuei.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcxmfzgda.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkexsqgl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gljjjvusy.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhupsjjs.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwskyzlzc.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxwwtfx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxsbyxem.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdqptmcb.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbobpoioe.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwaaxrpb.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoavgpec.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzwpjikk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlfiwpiu.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gphixtcak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gznwhqcip.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvqjluca.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gademjdzu.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqauwlho.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnypfwzoe.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/guqoqtvjf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclteazqc.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwezoipt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywbuyppm.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/giforlqvb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxeeuvfi.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gekjqvawr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxymviok.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmikvhxof.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckjkvblh.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gdnpmdtok.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddmoefjn.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gjupiysap.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzplhwul.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdwubywd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/griooanrj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gholirktt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gwmedylnp.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gxirzawao.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/glizrooan.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/giexvdiue.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvbvgufx.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gvvjbjklg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gizqynsic.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/grkksmaiw.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gbzntainj.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gfhjspxmh.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtlirdeqn.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwqhypbr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjplwjzt.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsnfuhbh.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmtdbtjh.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrsmjiyv.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gcswkyvdg.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gmtmrwxrl.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gdmgbqpiu.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjslyrljf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gabgotgbd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbusfzyf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gamdlpwjr.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtxxvdaa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmajcvun.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gvresorod.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwronagh.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqqgyrop.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmagyzvi.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gyyjbcolk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjbbatjfo.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gplkedzcl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgnsjhxl.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gfcioqiek.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdjvadtn.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gtxkizimn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gywmsjegw.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyouxdnuf.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwvmbuwv.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gbtmqalka.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gcwcvqojw.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrrumtrg.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcdcmmyi.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/ghritthgb.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gzxoifygp.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjasiphwy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/ghharfttd.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqkvjnqp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gzohcwnie.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gfcyjfcls.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gykmsfist.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/grrfkhkmf.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmofvnze.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxgtjnkj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gngztnxhp.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/giipxrfwv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxsywybc.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrquhcoa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gladixdpr.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/ganjpaisp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/glcgebqym.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgevkhcl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrebkbbb.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzblmnbyh.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gotvtdtgl.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gytuokfrg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdxhdiqgd.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gqftrazfc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gaviankko.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhleunsp.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggndyaaiu.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gxpayjoyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcfywzaq.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gwoiyzqgz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnbngttzg.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamnvetca.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvlsbskl.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gocpatlyq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwghigmxk.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/grnhvvpgu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkfgavoj.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdoqgosv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/glkzpeepy.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/guqwjlkpp.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gcomtkcty.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gnjtrvhyi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gaedryffj.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlwhhbkp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpawvenws.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/goyrclekc.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/grgxclzij.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmyorplv.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gxfpfrcpj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzacmwidh.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvsbjuekq.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtobkrzb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqardwopl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnwwjgwrd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/granpxezt.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gkztiggkz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteprmjal.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrofnwkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjautsdc.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grcvmvsqe.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghtlsppbx.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbdlygzbv.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gdqxsgclt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gprfbkvri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmexytfb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gxnawnhnm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gozozewrt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gxndhrjzk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gozvaieuy.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/grsownjrj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiujwhtk.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gltwvtdsz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gtvrwkkyu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgjfkwln.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlcguiwi.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdgbyjipu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gorxgowae.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/glqazvwfv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gwazjbcsr.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfccekdr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gsqlheyis.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvgsvbtr.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqckgkmue.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/grvadarmh.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/goswoupou.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gowhbymrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gxmkdgule.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlnuwhdp.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/graosgcla.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gryslxyst.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqkbiefn.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gtecnikyv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gtdujkxqf.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggioazywc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gjswlpjad.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcsgtjml.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhryjdqx.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gpoodyyfd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwoqvkcn.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gszzlnofn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gydgksmas.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gigmkvzcb.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgmxwtnr.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gddixwoaa.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gqbfcbstq.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gizldsdzc.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gjfzoesau.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtalgfrkj.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gjyhqmief.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfxlibsr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnrrdgzr.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gxflynawg.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ggeuhjgjk.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/glfonsdsq.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlrhylsl.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gwhywqmwk.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/ghbzrmvxv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoptylcv.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ggndohvra.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerukgfzv.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gfsvphvdg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjdgogefz.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gwdynycht.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbqlgxhct.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/givmasuqx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxmyjdeoi.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gouvuotpp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpjguhbv.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptzxuoiv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtmqvjip.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/glqdtoghb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpcyrptx.sHtML


<!-- 参考信息 -->