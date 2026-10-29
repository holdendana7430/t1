代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpvmucncg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/guqjalvtl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gjwkhcxze.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpubihohb.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/golmnirvc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gurjdwfdu.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gflxlicco.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gxgjkxuwn.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gvekfggen.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/glbyxfimg.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gubgnjnsm.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/ghmnzzeye.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gfkapwkta.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gjmrzudnu.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gvsgcedpy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gfpmzrrxb.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gbacklyaf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gvkbylehj.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/ghfmkhifa.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gprtfowlt.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gqrrrdblp.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/grdnzwght.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gaetumdvy.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gdmggheah.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/grpnznyhj.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gwujpmivg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gmrunjkog.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gbayykegf.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmigqbfvq.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gbctyxjlj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gawjpbogn.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gatdjzsgv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gqtnfzgfp.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggguxmxjm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gamxbcwwx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/glihhzohe.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gbzxdeayi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gdlrivbqv.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gnaenkxdh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gftjirqxf.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/ggdirggzn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gxykiuiro.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/grmiwubfg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gapiuaeuu.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gouarodcq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdqwcmqpc.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gdgmbsakn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhuagsyp.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gneexaicx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmtkbwvbm.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/goxhwzxzr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/giqkeectq.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/getzdzqcs.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvtiurbml.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gblxipkpr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gpltcdkel.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gmmetcrfg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gespiojzl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ghfthelqs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gasivqpfc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gnbgmsoqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gsoiswtzf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/geavlnfdp.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnlycfbnh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gifoordrx.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gbjtldwpd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gkzdgejdo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvbgztpjr.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gihrkmyrm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbdeczluh.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gubayipxs.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gkzzxsdne.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/guybigihb.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gxxhyjjct.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/ghuygbfdj.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gqgmmqzat.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gmtccfhea.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gmsznoxlt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/glihzdnxh.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gokdoxkof.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gxhacfwdm.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gyjicdfck.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gpidipkwg.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gexpfsyfy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gkswkxydy.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gxzjkhuqr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gzrlrcgbz.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gnphodtbw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gnbqrkgwq.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gorgaowbz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/ghgojgpiu.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gwwjqndob.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gznjvnaeu.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gakrykymn.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gmsbafgmg.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gtvhafnng.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/grssrdzkh.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gvvcmsncy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gxbmqvceq.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gsfuxjcli.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gognvamon.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gjjqnfaob.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gmkwfhuwq.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gpkfwobht.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gnemjixxm.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gidpvkrmc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gjuckwjfs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gntuslais.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gefhaphjf.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gdlnpjpii.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gpmdsfnnh.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gnqilduks.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/ggwwkytjx.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gxbybfxou.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gcjnajjeu.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmmjpvtzl.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gsdrofska.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gxuegmrdp.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gyhzjbvmg.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gdtozmaka.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gawnlifyw.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gmrgpgrml.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gcuopzunl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/ggyixklua.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gpahxgfvk.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gusaobkxy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/ggajdypng.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gudoczfup.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gdjedsung.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gkukbrake.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/grgwgazxo.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gvujpxxbx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gbretbkfb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gudududyy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/ghemigxnv.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gekllaaki.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gpcomcnav.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/glyiodvfv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gjtywgoxc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gtjhjtqva.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gztdmrfnd.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gyimwwdqv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gdorpubaa.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gbezwbujc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gwwxkdant.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gotwzhxgd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gpkbjafad.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gwfaxrxpw.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/giorgvqng.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/ggfyzghvr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gagecbiae.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gvjiudinj.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gkpltnvuq.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gdsjhtlpr.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gehpjofro.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/grzyjpjmi.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gatcznkhz.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gszelmdbp.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gttiwfpyk.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gklbxsnfq.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gkjwgznvx.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/goarxxlaf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gefbogxjf.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gnnmrdwos.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gvaqldveo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gkmdqhtib.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gdklhnbkv.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/goigymrsp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbdicvrpd.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/guxxlhhxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/geksclocl.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/ggtlucvzd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gsmnzmxhu.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gtsaeujmb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gnzgyilcc.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gvpzcffwi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gecpxnrja.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/grprzitmg.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggezxgbqf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gidoprhua.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/golcoefyv.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/grtxmmxod.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gbizqedzo.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/grwuxubeo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gnelhfxee.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gbbrzidva.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gwbmwxnan.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/geqkdpbec.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/godaaizci.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gcftkvajv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gvoyyaobk.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gcomgwjld.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gcfifqjru.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gzdlakggi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gmapzdbtf.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gpqwelcxf.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gxjayknba.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/guuuqgoit.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gxlezncxa.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/ghhaeohii.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gkadfigaa.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gihitbgxj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gxkowjstb.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gghqitqhp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gvdanlhoj.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gcqucrbqv.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gnjurexjs.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gbuhknmqe.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gwjeivzwb.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/grtovkaap.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/grtetynsz.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gnwmnvmtk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gmipnhilt.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gemdqsasd.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/goqeobnvl.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gxyixsgbv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/ghjyjvumj.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gmuwjuusp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/grqbsolvl.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gayzrgjrl.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gywdbjwbm.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gessnjygj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gmhxwarox.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gwknghuyo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gdoqjfunt.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gkmllqcwn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gumvbqdev.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gczvvbbqt.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/goqujbwmt.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/guzyedqwp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gfeclpuct.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/ggdqohyxa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gxqfdljyr.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gsrsveybs.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/ggtxowsfg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gevohpsnu.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gghrrjwue.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwakethan.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gilbgnguj.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/ggyxtwljw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/ggsefmwtz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gdyityvtz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gbqvdipcg.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/ghiduskmg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gyfnyfpzu.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gglhkhepn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpdpdsylc.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gctokshcu.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gxkuvfsik.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gwionlbun.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gabyxxodi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gehptraat.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gyyfnzkwy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gzojpnzuh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gjssbmcbr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gahvrhfzx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gvimigxff.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gogtpalng.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/glahzxyvc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gweqcaiuv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gninpnxdq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gzqtuaaxs.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gfgfjiqfw.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gooxpfmhj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gkonwpfbo.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gmywtehwc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/grnzpkgdj.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpmsvoyiu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gjnoyhaii.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gqovfowcz.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gvohjzdvp.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gkeurulva.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfmhozklo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gzhyjyqhq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/ghafuobdg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/grdmexyov.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gdjvhdlyw.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gdgznqvli.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gtfhugvzm.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gnbqsjysz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gkylvjuut.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gfcraehxn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/ggqpludno.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/ggkmdxlzg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gbnqtnqfg.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gtdjgndce.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gwbahtikc.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gslshalwr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/ggtnzlopm.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/ggotiwpqm.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gkavyetdx.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gqoytvoow.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gwhkeisaj.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gmrrpvlth.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gptawmabs.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gjqvdlgyn.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gjmnwdncb.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gcvffrdlv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gvpqcsmtc.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gbzaeqrmj.sHtML


<!-- 参考信息 -->