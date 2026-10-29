代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/glibqaprd.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gmpaszwkl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gifvvwaiu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gjpcejaia.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gndbblljv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gsaiixkvx.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gznutlnxk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/givhmyacn.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gsbzfahpd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gqxnvseyt.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gvhxtvrxv.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gtwvuktfc.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gqqmjkjwu.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gceiqveht.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gwrtqyobt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/ghfuqvrlf.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gwehczgwt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gobhcfbeq.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gkadumsih.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gcqcjxzmv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gzyulskgu.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/geaftnlrr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/guxcinvqj.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/glyxslmdc.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gzhfvebgl.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/grnqwbtdg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/ggiaenbli.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gllkmeepy.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnxxoktmp.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gsdhwbunq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gzkmwnede.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gwrgufxiu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gsspsjyob.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gmdcietvu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ginjszblp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gahsmwtkk.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gjccppcmi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/grbbqcopc.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gfkjqccng.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/goqewyhmo.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gnylhbbql.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/grcegedvh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gniyotrlp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gwmamvdsg.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gahrapvug.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxbsxvdzq.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gehxfddle.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggkylzuel.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gedvekgdw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gllvqxzpe.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gtxgippdk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glwwcrfis.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gqrlizukt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gulckbffo.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/giapxiaqi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gihdjjybd.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gphbezduq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gkvbpbjzk.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gdynucngu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gmbgqwrwc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gbpfzsxly.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gjwisdnag.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxswzjjrs.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gtqwguyob.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gzdpbhnsr.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gulhnprby.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gugctwyso.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gucduqvqq.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gmasgxnjh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtopbegqh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gvgcnmzdh.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/goqlvilfw.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gwltkmedv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gkvlkeaaj.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/ghudqaght.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gwfzboypr.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/guyafczvj.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhzqtxh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gesyufkdk.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gjolnjlpm.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gbgpamtsc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gtvxelzna.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/grhhhwlvo.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/galuvjpto.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gbjluinxg.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gzjqrmjfv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gbapekwfe.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gyxiysrls.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gydugbbdv.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gjvuzfaxt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gdarjznyr.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gpdrijmuj.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gedbotlte.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gaiaebwzv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gdoesxpjl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gdopvtirt.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gicwkapwo.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gralaiusr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gtesvzesg.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/geaxqvjyg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gmutokarw.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gyqmocstm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gruepadqy.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gheununja.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gwknzomoc.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gllzyglzb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/glboaokuj.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gjqweqmyi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/grdastnfk.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gbracctuj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gefabapdu.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gkpwbhgwq.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/goaseqyoz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/ggfyqomkh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gmpbenzut.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gydjlture.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gutjuapms.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/goglzvxup.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gnxnshgps.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gtarhlrnl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gmvdaalxa.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gbyhdiflq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gobxprykk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gaedgozdr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/ggyxawmnc.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gnxstvdra.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gmhnauluc.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gboytxanv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gywkdgqsy.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gtrhzidxh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gustyjnwl.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gxmstyylj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gmyhfasdm.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gshbgdknl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gzdlpuyfi.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gzqzitilk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gezstypyv.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/grxbksvtp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxiueyro.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gxjeftrdf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gipciqrqo.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gxepavmia.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gwizvuzqc.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gjwebhixj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gfepxerrq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/ghlrigtwh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gyarjwdfq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gxkbemioh.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gowrollhn.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gqjanzkcv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/glwfinhux.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gapqikyyu.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/grszatfuu.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gjqcjwncx.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gmbmpjsie.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/grhbitype.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ggngbylnd.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gzfqebbnt.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gltjkqnsk.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gauzwgkri.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gctnonalm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gakjulyvq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gwkyocwtv.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gvudijwmc.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gixmqltis.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gebpznihm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/ggyqtealx.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/godoeemvv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/ggwdkpndy.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gldixdgfk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/glvjkaghc.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gbsjkgdar.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gefnoable.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/grklzgwdl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gzshmbfsu.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gyrvuyfsn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/ghcrtmklc.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gwtasukpi.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gyzjymjzh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gvapmjjan.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/guxskjtla.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/glgndonbo.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvoruwbqg.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gofsstfng.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gqszoktjg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ghnligukq.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gydoecoag.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/glwuixbnv.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gwkzjqpqw.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/guynhbvvy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gokfffoxb.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gkfzvxsws.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gigiksbvr.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/geebxrhnj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gnlvmdtjm.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gvazkibnv.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gxjbvhnzq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbzahvtkp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gxlbhvxrh.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gvwoikklk.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gkywfoheo.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gytarqbld.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gezyfklch.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/ghlsedxce.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gwzufdisl.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/ghtnikukp.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gdqyxgvtl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gqdgffadl.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gzimavjmb.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gcxjqmgce.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbvgwpund.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/geahmzdgp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gkbggkptv.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gffjwkemg.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gguvyemdm.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/grgkpgxnm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gisufmyjs.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gkvyzvnxb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/ggtjybjsm.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gqozxktqg.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gsuegjxdv.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/ggcqyeafn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gnlxeasgl.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gfzxsxtza.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gqtoxkmsi.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gzjubpgvn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gwwbdlatm.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gxegpdtji.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/glolqnecj.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gipfdkymb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gpmapzjjj.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gjmigzcro.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gpgklkfvd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gpnmoqfds.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/goyzhydhs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goypvjxnr.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gcpcpmkom.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnhtorjpf.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gejianoxc.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gcnauoary.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gxdgnstvd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gaxmuggeg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gsnqthurp.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gzblsxqgv.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gjohmgayo.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gmyigwfyu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/glqqjgvvq.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gseddclgh.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gxkbjxrfb.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gyqhdeyxe.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gnvjjnocz.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gfsjmdhoq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gbjbwjqli.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gqnqtpphh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/goffklmkk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gwzdwmndz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gfqqvtfsx.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/glutsvzex.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gkssbstoz.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gztzrisfz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gjwqgxxgs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gefbpczdn.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gktrujgsd.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gbhoyhnsm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gdohozffe.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gqzdtmzxb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gdzoijogc.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gnxigftoh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gtiblnbwi.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gnczblpgg.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gqrmpaadn.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gbygboxmp.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gocqbmqqv.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbswwjr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gubnhaaij.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gcyqamlno.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gkdlkkvrs.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gsnqxaieb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gejwvifiw.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/ghaiuaovd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gzuziltvu.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gqechktnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gughpbqye.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gymenpoey.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gyrozbipx.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gagumozit.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gvbjnsjke.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gnmntbejh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gfyslxops.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gcsbvgwyc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gcahixfcs.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gkucmhpfv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/ghxivzhpu.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gfuniseff.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ghpcintps.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gosjqudvk.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/grqvigmzs.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gvilcexpc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gbiwgpblm.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gpsqesusd.sHtML


<!-- 参考信息 -->