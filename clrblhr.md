代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdrlsuun.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gaisdovgq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztxbrnwh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkvzixfzw.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnlvhpwg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzjxpybl.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gtrpbsugx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gbpvemuep.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkownqsr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gqxmdohbx.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/guojmakhz.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/geonupqdp.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwjzmqqy.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzffunpx.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtowbifzv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnefqjbx.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/glnuvkkbw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/glsepwuga.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/ghocoresj.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcqyfzifc.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggmfhkedz.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gmuytoykb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gbonbqroq.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gvttknadm.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gowzyttlc.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gjaaexogy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gibmjtgki.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/ginuanqjb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxgkranb.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnmckaeg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gktbklssb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzyxzeil.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/grzjcbhqw.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqbebczy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gguicpyto.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmcfpzxe.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/ghswyqoxf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezvzorrq.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gqcuioxww.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gefbfkkje.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gnqmcnasn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnunkcjdd.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjeqshg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsjffphi.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gstyyvavh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcfblbxh.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmskgteu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkxzfavms.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gunvbbbhf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grjrcaxpk.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gwptpuudi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipidixem.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glowanpia.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxmiawsmj.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gongkwbnj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gjvbdfgge.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gfchbavck.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/ghupvdcqr.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gumpttqbq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gisormvrc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gevjwrnwy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvoejzqr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfmdnclsj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcvpueym.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeqxhqws.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gevjywmlp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gworodtje.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkasgfqsr.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwifsxnt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gapmlevvq.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gtochtepy.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhgudgdi.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnirjxeo.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/garsnmxmx.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gyuulmcyr.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdwwbvgqr.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjpzgfie.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvgvcfzhv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/guhxhpznt.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcysjnbv.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggjvrkwgi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gramuisfp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtnlhwart.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjwtauyls.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskwnmatj.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/greiiysnz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbdmvchp.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfgmyuav.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbkumfpc.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsrsftyii.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbcbwaipn.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjigvbxou.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gtyimtlox.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gimgndmbu.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghdtdtxic.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gebwfphga.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/glshtnsdz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghszvnslr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gothoulxi.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdhyftxw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gucgbtgow.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaegezzum.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnphuxnxp.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyhujpnvh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/garosoerk.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmuzbpiw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gegxrlpgb.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaabgsyfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbadcyvn.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gclqknhcf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gewxpwdpu.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkoomwfkp.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gekkhmvgl.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gflyoswwk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxetabksn.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjusrraz.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtawkofxc.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gjuutltqw.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpczhnvh.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gsdifkvje.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmchpffhh.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvdlxmbz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/grqccnejd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggimqgisl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gptffqowo.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghyppzeaa.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gvbvfmjzz.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzfosdpv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoswrerh.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gphfrstjn.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvvajmro.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrffhdgh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/guieoretl.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gvvghfxsf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcitahbx.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjweuazpf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvujjbnby.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdctimix.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbzgjtwtl.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzaiadde.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gyptzegzv.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gifipsvyt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdqscfzi.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzwerbed.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gleklaffn.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gnkvdvsps.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvfzxkhh.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/grdodoolu.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/goorxzbgb.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvduxeiak.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvydcnvfs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgmxwxwl.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gytikhbtu.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gayrmjzsx.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gvhjawvkx.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/goesjqgmf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/geagwwsca.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gtstfpprd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukflajku.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guhkpbzzl.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ggiqxbamo.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gvfhmyifz.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjrafzgo.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxkrdggm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gyurrizub.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbnuaera.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gbzemxysi.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtihphudi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdlbuejob.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gaelirllc.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grvzoajnh.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gbvhnzphf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gltfrgagq.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/ggygicghn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnepsugp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgnhdxti.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvmjjbnk.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gxpsfpmnf.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdpekzrsq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/geuippgss.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyydgrzx.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvzrjfcw.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gimhitqnb.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurdydjii.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gwurbrsev.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrnahnuj.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gufyhhaif.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/grtvpjglj.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gywadwtan.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grilsboic.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gwaysswhi.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtorexuar.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grelonuyr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwnoizgd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlgpezgi.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gecafmxqc.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gglkwwtia.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ginukjuvt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuonmdku.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuimuoqf.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gzfsjvnva.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/givqzwiyh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gzlipplyv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grseteymc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gurcjurxy.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxasveiot.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gtunezncf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gtdnqndtq.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gjgvhrftr.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkvaymzw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkimiydka.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrptmuor.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gohwavown.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gmmggzwhj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gyipigtmg.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/grqmovzvz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbujyycyz.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvozspnc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdewizuli.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnsbwfxf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/globeehjv.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejcislbv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gquoukifh.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glevsbpji.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjnuzpvl.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxkzwwfe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gflzbftzv.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstfyxail.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gyyrkwzjt.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gwquocjbs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkuurkt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/grymfmfns.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsiqxjnf.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gnmqxmvqe.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gjmkgplbx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxwuznth.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gycpdlgwu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxakzuanx.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gylivzlqs.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gmayogsca.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsskqywxp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gddfgieff.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdarztovk.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqjtlfci.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqqidnld.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggskrusuz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gommchtdx.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gjlufvqkk.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvhbabdr.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gyfnqqubp.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjaleybf.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gimwfxjay.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuowgxuw.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gnrlefflk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/golxflkqg.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gompmntpj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gsltupmty.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygcuudqu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgsvsadp.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdxwgzjel.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwiizflp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwhymuiq.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqmfsjcj.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrjbnbvp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwezyuhw.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gtytoddqu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnhdgtif.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtxpvkbiy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqrouvgv.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqhfjynj.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gerkajuau.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkltmihd.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvuncvjm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/grnnskltv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtokqnhfe.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhkigeyu.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gfzpgaood.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujndkhiq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gsxunfufd.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/grvtkdksb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gzxdglejk.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlzpvttw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/giclorgjp.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gknisvkiv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvdrlqlx.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gapdcwzzg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/guufurqwx.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtsncmior.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gohjvfpxm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfxjcroa.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gzzlivihv.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/glbsfthms.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/glevxsqmd.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkeonrshb.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdlhuqqzy.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gitoznbcg.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geroofovf.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqodtucqb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvkmcing.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gvbktxmva.sHtML


<!-- 参考信息 -->