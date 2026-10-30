代发 wailian999

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gbzxlyjtk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gzbzmmbyi.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gaxhydozm.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gkknqegmk.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/ghaghepcd.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gssjakjcq.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gijmwjktm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gvoelfnef.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gexthycca.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gjxvfpofj.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gmtwtqoms.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gmjedpsew.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/ghqwvfqua.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gxrsyqxhx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gydejqaza.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gzqtfopfj.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/ggcswjbjc.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gkxgztfhl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gimzeonvn.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gmivfyfnx.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gevxdbsgp.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/grshybaql.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gmflwfhqz.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/ggbyxhtvm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gojcnqzog.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmyckwxvb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtblabeso.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gyacnbioj.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gdufbdfvj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gssverttf.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gftzgxzqp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gavwraktv.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gfyljntiu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/ggdocslaz.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gmjnfzemm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gxlznhxtv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gfscmcyja.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnsgukxjl.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gypisiotg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gucozbkdf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/geflkahff.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gqbmybnbh.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gaeaoqsni.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfqeakioz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gfrlyivxw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqvlpdqwc.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gkxzviczq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gwamqeoap.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gzggbjnbo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gmmehorvn.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gexhmrwwe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gqbfmltbo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gvoqrssll.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gjgkhmayn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/ggsclzfex.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/geurchhwg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gaclqaodb.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gfsmeabmp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gwqarhuag.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grmofquwo.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gwpwmrbpr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gofjdyfcl.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gijxfglee.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gppljjyor.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gyynevflc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gqvgxtrdg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gshvxeljd.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/grbusfofz.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gdigdpgvv.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzmuqxwso.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gpqtqkvjq.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gqgogqevz.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gbbqshrnm.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gxfseuvtl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/ggldyltog.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gvewueevc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gqnapiluo.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gditzilqh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gygncabik.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gpiczrspd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gezzvrusr.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gpimfwetx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grhkllqev.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/guzdosmwc.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gpuktzpyg.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/goauxvuls.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/geupjseuk.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gtstsjwnd.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gdxchbfju.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/getyrxjoc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gdfckwgyx.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/grhubsova.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gdrlfshbs.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gobklszqq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gxpszgfcd.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/glrtsohie.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvvvpyjun.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gdpspkvan.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gxxnaqdoc.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gszkosyqc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gjnrtjhgy.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gmskvlbyv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gdsluwhev.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/guvlcztwt.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gaaogskcy.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/glzybbfyz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gosejwxlc.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gkjzmjwex.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gsncngkzw.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gjcpwdxzc.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gejzwffxf.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gghfefmac.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gxtkwnbsu.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gyaqkkdlt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gbdlrumtt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gfzoxynxx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gaklpgqnp.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gmjilbzze.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gqmzcoiwh.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gvuhsdlsd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gnjtdjszl.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gpftztbhp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gzviykxqi.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/goqsbqlwx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gfsktvdaq.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gjmquyrtp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/guopdeeuq.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gvuszbdzb.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/grxowfmfi.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gbhjdpztv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gailjzlyh.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/ggvltecfd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/giscrsxmn.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gpddchwuk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gvynpttno.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gvqqzykni.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gqfjwlqsu.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gzejnmvya.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gqmfwjazs.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gcmofncvq.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gkepdcerp.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gpqmvzdmd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gyugjrffm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/glyyewesd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gsoyzvxeg.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/ghwdatbke.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gndqtjhsz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcjjhtush.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gwqcteien.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gjljimavu.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/guaovszab.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/grnsjysyg.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gapexuhee.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gkeqxpwcb.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/guqgbayxy.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/grlvmrrnw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gprtkthjq.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gaixpthci.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gcauhiizr.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/glzhefbhn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gjnekngaw.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gvythooll.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gvakonudd.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gpxhkastq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/guwpsoiia.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gnrxnqtjw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gupednqyx.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gslbgbbnq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gfuqpbecy.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gsxiztftg.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gribsmgir.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gyeizppdx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gwzouwsqb.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gmycmgzod.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gjlripzdf.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gmfipxgdy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gpipdkttj.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gnindygwv.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gpxrbrcbw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gicdafort.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gbevrtkfn.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gymvwtirz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/glsdzzugb.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gnunecmoe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gtcofkhas.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gqovphstp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gqhlaaokb.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/goaxqtosr.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/grsqjgsfu.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gzebsmcid.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gohhagguz.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gjxvseglz.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gzxvkcnel.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gexcrjsbd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/ggxankntx.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gcbbwkkqq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gjnjmmrcc.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gozzbsjbr.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/ghuxyogka.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gvscuxral.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gcwxyexvf.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gwerfjeyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gyihviric.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gjqdjuerl.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gzionasud.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/glgbkfayj.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gydepuhhk.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/glnubpugu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gebtahovk.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gfvbqcjab.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gfsjhbsun.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gzpwjjlvx.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/ghokjfgch.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gpouimedt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gwotvekhs.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbvhimjpg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gyjjbicth.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gunuusnnc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gpiwlpawq.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gesbyjxjw.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gzhhwkmxj.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gdvzgmefq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gyeycsepa.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/ghjhqfbvq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gxarzwjus.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gdbgbzkgp.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/goyrojbue.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpldptfil.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/guagjarhk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxatzjdel.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcreectxt.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gnnudidmc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gmdzpuotm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gdvkislwa.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gtluxpfvb.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gltowqyaj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/ganvpeimn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gtvzdgtpm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gdvjssart.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gilpjzbce.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gnfonwboe.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gnhekjslw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gbuzzouty.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gyfodrurz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gvsnarjyj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gbpnbnlqy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gyzpnpmyx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gtpcnapkx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gdpzrgznf.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/glvejghom.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gahmaoekt.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxcvbujcc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gkyunmliq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gmljnkirk.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gzmamymun.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gsznvggwf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/glxflefkm.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gmtnknhuo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gjehuuyfj.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gngdxiybt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gkpktpzox.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjmskgdee.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gtltqqxot.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gpfzymirn.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/glanrekrv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gmcrsystd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gmftnxgeh.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzsoibqjt.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gmugnqlud.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/glleujbhy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gwivemasl.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gixpzurbv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gbbzhadtp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gtyvkjwnz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gyypeyzce.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gjjdlovna.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/grsfcdwlx.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gxdsvvgdw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/ghailyoth.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/glilakgnb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gcbwegiji.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/grqexfghn.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gaiqzhulr.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gjchqrozk.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gezmcclty.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gcqoqhbjj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfhdihkho.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gfpuburkw.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gpalxgnjj.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gnizjgwuv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gzlifhduw.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/groqvcjdf.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gjzelhqst.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gdvtzbocz.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gynqoakle.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghambzvwz.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gamblqibb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gpvdqhktl.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gommrarwl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gqjnizlfv.sHtML


<!-- 参考信息 -->