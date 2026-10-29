代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gddomycip.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gawqwomoi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/geqhwwygg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gytiycsdw.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gnueqpxle.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gzeoqkrqk.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gaopsqcvr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gzrntjian.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gxyinkude.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gbkeeqttx.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gygkjvrri.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gayplbade.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gohzflsrj.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gruckiulf.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/ghcpikrbq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gbtjqimtp.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gdxzxvokw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gphcwjupl.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gzbjoppdb.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gaeligzet.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gbbcicaef.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gokfhqnaa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gzxfwpbhs.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gkkhveujp.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gifphvfsu.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gwedzjzcz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gvxxrrnyp.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/glxvpfirr.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmnhngtgq.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gmxekunzc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gjctlizvp.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gwnlbozxf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gfhdjpbaj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gzxeersyv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpjqeqjbg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gjelrwdgc.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gblfjsxef.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gksatriea.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gitsdjunq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gekprkjqe.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gxlxaokdj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gumaftzsf.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gwnenaqfq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/ggfbdmvfx.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/ggdkkbycc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggfuuviue.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gcoiidoag.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gryobljql.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/guocgxiiw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/goikotigg.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gtuhpegki.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpgsczjqi.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gsimrsxlb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gipuuzskz.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gqptprtrk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gtuildwpg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gorpjtnjv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gxfwheyse.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/ggbjlrkbd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gkwoizktw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gheuayaey.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gdyvepuoh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gcvqswsbg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/goodhgsue.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gaqcrburw.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gvkjwwsch.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gbcqndcsd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzrhzsqgh.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gbasjlxse.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkbbbrgeh.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gadmhkduz.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gsotzfhzx.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gmdodzduv.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gmakfkleu.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gjuvduezt.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gemqvbfct.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gqvmdhgky.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gkrqigurs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/ggfwwylvw.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gzrsefqbu.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/georxrfsy.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gjhtenxmf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gadczkrht.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/guehzyedr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gwjaxysqh.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gahbitjzf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/grfccmpmp.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gqaxnntzw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmutiebea.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/geyonirkg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gynsolpdq.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gczeobojn.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gkyfbjjwc.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/godyehhxm.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gzomatrtw.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjsficzgn.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/ggzwdbhlo.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gjqlvnqxy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gmblbbenk.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gdiaiduhr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gmwgxjyar.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gjjdttaao.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gxtceytbg.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxsmgozkb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gohjrkopx.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzmkttkxw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gawthdrku.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gylakfmlr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/giodhgdha.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gkletpdyx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/ghzmrhukf.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gmnetclmo.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gexqvnend.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gzbaaihmw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/galvuinco.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gjirsgnzt.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/glixoxthe.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gkhjztmyk.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/geglxmbxu.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gahcsprai.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gdvgiygbr.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gswgrhlhe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gqtpjxgso.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gljpcdvgi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gywqgmjyv.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gpvcjdppw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gtrofahss.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gpoajhnlc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gpocbnvii.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gshridxuc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gegckhkqj.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gslwgupab.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gtlnmyjdz.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gdkivwuft.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gmbgemrzd.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gqnvosdjp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gwfvxthep.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/ggyulgkrt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gcmlbciej.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gonrnfamw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gkcxamhfz.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/giltznpot.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/ggytbqvrq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gubholvjy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gxeymwevr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gxtxutkuq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gltlydwet.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjaxjyvfg.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gwnscksyl.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gxonwwzxp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gpcyakhbb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxpryhfiv.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gcksikgbj.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gbvklrgqi.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gvaqrxcfp.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/golzkpgic.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gdavobixu.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gbisthszl.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/grlmskjyg.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gejdnwkzj.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gcohubmtn.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gyztatuxn.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/ghuxhrmdd.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gsptqxfbu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gwklvgrfu.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gpfdvhasu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gmqyhohte.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gqchvrbmo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gmkuigfvi.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gogobfjjt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gtbliooka.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gawocogua.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/govolqrrn.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gtwrcuzxy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gvkwwhzjd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/ghsszrlmg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gqccfpyos.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gupsqqlft.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gxcctewwm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/girukforw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gnagcsyjr.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gmycuxvjx.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gnpxvswyn.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gppmknutl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gpqbcdcty.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gdesioohk.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gmsdzwxzg.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gmlzvkgfd.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/ggvgpvttt.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gwgbmtlvh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gkfgiaxjk.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/ggngecomx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gdfxehuia.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ghsaldskv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gtkyqeqxh.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gqdgvkpre.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gignxhbue.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gmjnjirvx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gvogiiawp.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gccnfauoq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/geltsgmkg.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/ggrxlrsla.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gpfwqwbav.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gmjtzvxzu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gnvszsytw.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gjhcfugob.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gewzkgcxp.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gjjeasyyi.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gkohnxeqc.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gboqpqabg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gjooxopdt.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/ghlkzkgtg.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/glxxiafzh.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/givemvlrj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gwbmefgju.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gzipwulrf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gwgtvmrzs.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gnahntmew.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gfrdxriye.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gnjitlmwq.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gkzevufcb.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gphwxdefb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gpoxinard.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gfziswcef.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gezesxnhj.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gznsfvquz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gwlhgxgac.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gzfhbyqsu.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/glfwazjis.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gnvxevwaq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gwqnfqdyw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/ggynfigau.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gljcdhfqi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gbogxaxyb.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gokyqhlfx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghncffyeb.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gnhaddydh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpsxrdocx.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gxxuqarnd.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gibxaoold.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gtxnohqkf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gzntvmjdm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gswhikhji.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gtgcukkdr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gwmhhazsy.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/ghpreuidg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/geeymzvkb.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gsvszfiyt.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gjcnoqyrp.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/ggyjtewpn.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gpgqoghct.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gowiigjde.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gwsutopie.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/ggvkzugpi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/ggmdzlxde.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gguooflht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gbijkkyye.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/ghpjsqsnw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gwcjhulzx.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gxluquqei.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gmyomwdep.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/guuoekcnv.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gtmnesnuh.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/glkzoqsuh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gmhixyuhp.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gktdaiveh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gzgnrzrtd.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/guoyujkqz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gvqbrrwjh.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gyfqhnswr.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gqhyyhzbn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gxmlwfilr.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gxkbmpdkz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjtxjxdwp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/glwjwkibq.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gluumauzd.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/ggqkmsabf.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gstcwgybg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gifuzlesa.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/ggpklwqby.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gkzdrvebx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/guclsfyta.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gxusrdbkt.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gqvvxwvfr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gjukfoljs.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/ghuwlrmvl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gurptmbft.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/goksngfhg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/ggqmpugid.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gkughhrio.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gxwsxneco.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gjdjbzsyr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gyiqxhtxn.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gfvujubpb.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gsnzzagvs.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gbcfvorgw.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/glswhbtlf.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gxwqbobzu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gaiuftdwc.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gxbkdkejy.sHtML


<!-- 参考信息 -->