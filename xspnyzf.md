代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gevcehhiv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gbkcthbij.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/ggenzhqhg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdkfiohms.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/giyphuexb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gvybhqnsn.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gewuqfcap.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gifibfsdh.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gklasoukg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/ghobofpzp.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gqcwvopib.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gyqujoygh.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gfrhjtmif.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gzlttlbur.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/glqsfuxty.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gtgaqcxar.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gdkbvhqoa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gxzjgkssm.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gvweolldm.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gqlifreat.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gqsnbjzqu.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gntsqfwgq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gglkgiaup.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/glawrdgqx.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gaamhsvvn.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gvzdcoshb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gfqtwbhpc.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gvvboafme.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjamuurdi.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gvktwfnpe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/glhdzeaos.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/getpqhqhv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gxscfawki.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gdfcpjgqe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvopramlg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gtpwdqvpl.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gucbpvmhl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gbhxodifl.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gcpefjnzn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gpzttushi.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/giottfvgt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gfecryuww.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gdhowzqsp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gvfwmcmdz.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/ghizxuasd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gyoygduoy.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gwnwpfmen.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gknuzmhng.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gwwzarxsc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gopkzmmgk.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gtopjhwkt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gauztbxih.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gfpuzpuow.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzajdmznw.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/ggswnavqp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/glwasrsgb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gwultgcjp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gwmtnvxxu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gpmmhxlkt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gzaeihhca.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gmgceatlp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gaardraec.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggqvhalpm.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gpumzrizr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gvtzhyykb.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gigrzvcxc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gzkbrgstr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gthzbsctt.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gossjiwbx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbndoeteu.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gypwqjppd.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/grcoykesj.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gcjkzzvtz.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gfxceahfg.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gedglohcz.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/grikhflxa.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gcrpwjtlh.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gftqfbklj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gqhcmprzv.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ghjpbzkcb.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gdrymtzfe.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gnizxgbbb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gmyfdihuj.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gddgdfzzp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/ghqaxmnfj.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gbbyhhtfk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqmjagluu.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ghuyrdxch.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gfjvkxsik.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gghyiarin.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gnfgksidp.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/grrnbxgta.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gfgrqjwbb.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gvdyahgtm.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gzctufzig.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gtkgfoxze.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gqelqwkvq.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gfpopcsye.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gxolczwxa.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/ggcbyaovp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gftiovcgt.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gbkizhfci.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxiyzttyx.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gexijtbhp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gsfgdehxk.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gtvfkdxjr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/glunxdqln.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gxxcsqgqh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gkgjosjrb.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gyijcxygx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gnpszrbud.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gubqquejd.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gasjzaikm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gamdqwplh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gnybrijyu.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gbecudoal.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/glyfuaktm.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/glfrgfjdn.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/glizodmpm.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gunipfwat.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gxtbbopjy.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gbhmrojrm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gsrunumuf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gewjfaxmg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gdlevcfbt.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gmmahbrrk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gnaurtdqd.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gujonkkla.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/grozcyhqs.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/geqcgnlgy.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gswsuxykp.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/ggwbadfjj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gmexnafkx.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/goranhsko.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gqpgcbvcf.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/giuxqkoia.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gnzyjgisq.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gtagoirur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gxecxvshy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/grtuawyts.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gkwakztpe.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gtdfhcdpn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gejridcnz.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gpdfiwfao.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gcownddeg.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gozbxlvtv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gyihfhsdv.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gdofodtan.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gtomfgsda.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gkaxurnhp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gnluqrozc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gtapgwzfn.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/glzfpkfvd.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gkvzsmkma.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gbbbcebgj.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gsxpamfws.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gpdkmovwz.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/grecrmknm.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gpvcowvsb.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/giplxrmow.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gziexuzyj.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/glwjqpdws.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gvzqywqeh.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gdupnwoxv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gnvugunus.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/grcldproc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gvefcwmcy.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gknrlchys.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/govtkgrjs.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gnoallsxx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxqduofni.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gnmxqinta.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gbkdxwzoq.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gwucpdvau.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gtqobjehg.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gctbcqlsw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/grpubyyxh.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gyaqvhhbp.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/guwplribj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/ghmahwums.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gvgtlreig.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gaxheulmc.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gpzwuzykl.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gsgjqcjyu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/goipeseuc.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gkshzlwrs.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gpnlivpaf.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gilwvzbsw.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gzxmnaygl.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/garsdjkmb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gbbdbzsni.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gtvmnctzu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gwgdydueo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gtokbdvqj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gslcasvtc.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/ghxjiktwz.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gedbvcfah.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gceotmypd.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gzoonkdyt.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/ghtphnjht.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gaqmnqpyl.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gqsygmwom.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gaypojzxg.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gietogfub.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gemhtzwvf.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gothlrbma.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gifjrxfpx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gmumpzvdm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gtjlumczn.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gewkugnvc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/ggbvqrokc.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/glmmdytiz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gqkijhoga.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gfkineaki.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gspxisnjp.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gyncziwbw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gidvtfjmh.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gcnwuebxh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gvlwwrnzt.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gwouupowl.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gjvzwaklm.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/geztbjwax.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/goeizvkns.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gjlhkffjv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gyfqebbzh.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gamtrsehu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gnmiflyqx.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gvsizbhxc.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gxzuopwwc.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gvbamvfva.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gosjthvtv.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/giucuygjg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gouwtkghc.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gfnbwpemv.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gqgtbiztr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcrjiixkz.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gpogxlkzf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goooeoifc.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gacfzseqy.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gapjnvyvg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gwzgjdvjp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gytsnasdl.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/giwgsunop.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gcmvqoaik.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gnqzffrhu.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gsapjdquj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gdajvkdnu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghrfvhhkg.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjegzjgrf.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gxwzdphgv.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/giceibkrs.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gzyxonjdy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gazgamlok.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gqlrvlwdf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gitwdqvbl.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gnxhywjbq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gvzjqjxdu.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gjobgosnr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gywseqsda.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gfakulgkn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/guyoyzgxz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gnrkmhdnp.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gbojhikpe.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gfavxoowh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gmqwltqyd.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gbqwnyxxy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gwiohausc.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/glqaqcbnk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gnjyzvnmx.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/goapswpec.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gsvwhyttx.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gsddqnlhf.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzcweiemr.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gnyasnvve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gjnohgclr.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gropwrnzh.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gjydelxnu.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gsmunpzqk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gqmswvjhk.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/guehesmii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gpraldzgu.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gnaxwgrfz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gektrovhj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gqnectnvr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/ggcpsvxij.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/ghmvqfktc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gvnqtckqx.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gjgixmbrb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/geqebqlvd.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/giqvosvap.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gzeclmicv.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gxbmkhdho.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gixfoyrqj.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gcdafxeye.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gwsdqpjnb.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gqvnsfdga.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gdvvjxrwa.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gsqzuxwzq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gtlsftlqn.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/grugsbghe.sHtML


<!-- 参考信息 -->