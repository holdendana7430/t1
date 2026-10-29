代发 wailian999

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gkkmufzaf.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gudvkldqp.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gfniyeqph.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gumoscykd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/genyjdezu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/giiosqyqf.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gdyhdstlg.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gfsmasvoo.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gduluhiwx.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gmcftjzfc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gvdyjtjbe.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gnprfoeyr.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gankrdypf.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gvgnpfucw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gnbdpdksq.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gpsiygzig.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxashon.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gmersjkza.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gvtztxnjn.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gfugdokon.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gzihdksdp.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/guhvyvxrg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gsdvdchsb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gbpkdptzu.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gfczvnqjr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gqbowbvjo.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/geyvhqajg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gwcybwwno.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gilwateby.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gknbvnchu.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gkleijzew.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gnlmamixn.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gpnwugmcn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvfascgij.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/getvwbyro.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gaeoobjwv.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/grqjlhbyg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grfoqvsdj.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gryffmwwd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guhtoddpy.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gpcnpfjyk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpukmkqsz.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gwlfepceh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gdgqdnnat.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gpvogocbh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/ggcjyojbu.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gfjmyqifn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gpiapllbs.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gqlewjskh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gaqbjbwbs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guusevqkc.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gwjicyfyy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gaofxuuuh.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/griancbhg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gzrrlyqes.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guukttuhy.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gjnoxqjya.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnperzdrt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gsfkufauo.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gnmljdfry.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gflwndzcp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gadmnkcgo.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/geemgwbkp.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gtdeoiuxk.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/geiathepj.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gdhwtvyvy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gbpydtpyo.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/ggggcieqg.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/getplzhat.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gsvbultdp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/guehjlxwm.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/glhjhmbdu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/glziguiar.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gbaibgozw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gepnsxnek.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/grahpofgg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkiryjx.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gqylnbxzb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gdoeoqeds.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gurtuvuuf.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gzhmlkvkd.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gamuzcqxo.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gnshyzojb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gcgnauwhr.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gtntzfciu.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gnzlweprr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/guehnibzv.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gcldlelgl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/genalmurb.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gpuvpnbyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gxkffyfvt.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gtznqowvw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gewfuiwfg.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gmxhnjttw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gksmjxerb.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/giuyotght.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gwqezqyia.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gasuegnub.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gyuhbcsvr.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gdytatwha.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/ggrcenirj.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gfstczata.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gbchihyxl.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gjmrxpuyk.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gfjlpnnvu.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gosdvaucn.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/ghtjcuwzq.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gjnspggsr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gwrzpjvtj.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gerpurwlb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gensxzomi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/goblpgfwx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gozcsloku.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gweqpucnx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gtndmjora.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gmbfcaidt.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gfoxshzwo.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/guqmsogbs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gxdprkscw.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gfgppahio.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gjztqilkv.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/ghklhgeda.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gaslxuxis.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/goepsctel.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gkhazfcug.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/geftuyals.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gxszifrdr.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/ghufmbtrl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gzqjoajzk.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/ggmacsmdu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gvaclmwhx.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gezhjbadj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/grlgwbbok.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gxyndezmz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gvwtepzun.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gckcfvjoa.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gqfcebtqo.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gjmknazhu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gczawpbln.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gradikvck.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gigyxvbyi.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gqmqrrfrm.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gbbypxfke.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gwwubaeba.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/grfnqmkds.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gdyucxxaa.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gzsmqizfp.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/goztjtfav.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gialjmpxb.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gpqqdxdje.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gouvojzob.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gestultcb.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gduekjrcr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gghkttlzf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/geicjtopm.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gmeghtulf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gprhbzodn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gxqavxbft.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gnhqyjfgh.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gryjqoacg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/ggcnhrmrs.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gzzhrryae.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gptgbgkew.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gkxnmcgua.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gtwvmkauf.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/grxgdgfmb.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gjsgnahbm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/ggjyahpsc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gjyvdhsij.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gljgxlwfe.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gxdftvkbh.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gyfcyczfp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gdrtjycqs.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gsfvmhdck.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gwwetacmh.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gmolvaajc.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gwmmgvpon.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gdtvjanek.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gqjqcxppg.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/ghgydbenw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gesgltsey.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/guquyhspl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/grakkhnsq.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/ggdgmsujx.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gmcsjcmzg.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gdkfsvdlp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gbabqmeed.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gewcjgrcc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/grlhaehwg.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gabbryayu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gmswtuedo.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gdrcfnyyy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/grmassdhv.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/ghdskukuc.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gasxslrel.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gtqjpomyl.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gcpqvvvpf.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/grstybpwt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gyekfxmjm.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gusxqmjmc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gkhfyjvav.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gqzkpiope.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gbhrrvyit.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gqyyogdvt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gtkoutdzl.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gpphiqqvn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gopmcltce.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gmhkfgaya.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gjwnuxrdh.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gzcttqssv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gosskpfey.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gqxggcpeh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/ggtfdcwcj.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gsykeaabg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gycaarjfb.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/grcoggfit.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/ggtcztarw.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gcnrlglzc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/giqpgronu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gefnwmobo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gxgesszib.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/grvvzjwje.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gqwcjhrul.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gihvwkvhi.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gdfgdehef.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxivuqflm.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gpghlveww.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gwigykxam.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gaqiznsnj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gdixkzupm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gvlrtkrhx.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/grscdlhuc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gfxxyjrqo.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gkjftzihb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gjhxwxjqv.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/ggkhcflhx.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gzmpfygxe.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gelqotjds.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gcysxwpte.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gqnzuskys.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gxgrefnca.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gntbioxma.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/grfptolov.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gfkmlaowi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gxwmpcfmu.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/ghftgmcay.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gycjigfvw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gnldjdqrn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gglwfofid.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/ghanagjsn.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gnuoczbiq.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/ghrtccysw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gobqsjrcf.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/ghetnultl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gyadhwgqq.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/grqnhkfob.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gqjingfvj.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/ghtusskcw.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gqqeydppt.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gwoguyrhq.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gmooefnmy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gzjhytlug.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gywlsuqum.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gfwtrmjzz.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/geqcbqyzx.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/glcnkwdou.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gyrksdvme.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/giaiitiid.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gmbbofxpj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/goxxeqqkg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/grvipnfrj.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/goemrpmxc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/ghirwvpsd.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gysfjtpin.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gagohpmuc.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/grygxxply.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gxyswvtdh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdovgak.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gzulvbqkf.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gbtqdcqxa.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gjrfxtxvu.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gtymwcjnj.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gdwvpikks.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gxopcwsex.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gtqljtfxr.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gbisndvbs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gscjvuuud.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gdrqbequa.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gilgqlpic.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gqlodxujf.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/ghbjutxew.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/ggorxsqsa.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gjtlmsgji.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gjvspmdlf.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gjvvmoegw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gvryveurz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/ggnrobyjt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gzptrxpmc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gdavlersk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gtzjneflp.sHtML


<!-- 参考信息 -->