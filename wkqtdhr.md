代发 wailian999

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gjgsibicn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmlutnpm.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gwywrvtky.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gamkmtfqy.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbpikpxz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/garavfpmx.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gkuasvffv.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/girtqxkzr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdswysyky.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/ghesdpneb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzckzqre.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnntpgewl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgjjiaim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/getpoojbi.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gwgmwuwxd.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/guqwhstok.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gypyxgawc.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gkgbgrmnn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gffeanqzu.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdphthqru.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glepmvhpu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/goignypyz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gvjjpnwfv.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gedxjenwi.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpcytkmu.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjnrmcne.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gfupiwxrz.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/guytliofv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gywvzeiwr.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/grpvaigxq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmumnwind.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gkucpkvud.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxftlgmj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/ggoflfetx.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgptdutj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbrqhyre.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnwudvnm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/ghqihxwbm.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrxqqlce.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcxpskpz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjokdyxfj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gantulgzg.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmeczxpk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcsfausk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsrruogyo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbdzsysw.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnfdbrlu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gehfsotcu.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/grsrfasnw.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmrxwosba.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqkxdefh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gfmepvffh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyunlrwx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gbfimckbl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfngqqwl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjyahdtq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdafdrspi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gthxrazzx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxxfebvv.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gihcwhlsa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gusdsweuc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscfkwhkt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gsekernrv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkmjbcbnq.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmrjfmbq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevrigjfb.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gimxcctlv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieofamtw.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gyvxvapef.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmnjbgij.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamzytisa.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcugzgqla.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gelfrpgjk.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkidskduy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gosqndnfg.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvidouun.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gupraplms.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gepkgbbpe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdexejskv.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeluusdf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhwtixqg.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjduacbkx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrqazkdh.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/glpepzrrr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpefqbie.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gbvvhrcvq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbgrqbow.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/geydtajzu.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/glcbxcjvc.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgfhrvsz.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwfyqbkbh.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuoaxsbn.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohkyrtxs.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwuzevovm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcsusqyep.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gjevxihrh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/geicspggk.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gwgsovzln.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnqtxqkx.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbuplyqmx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjuhmfid.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxxpvcta.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyqogrcnt.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnigxnikz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqynginft.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gloxflmpk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhxekfxa.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gsibfgmkq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklukdmvk.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gdtmgyqdj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwysjchh.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczrmdcsi.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmofmynlv.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyzbzzxr.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gprfzonfz.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdlnkjmtl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gehnpdcja.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhjofhmx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeotbjeu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/grpvehjvj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gayddqlqh.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfdgguwjj.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/grqunslxb.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gbafwagoa.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gmdmoflog.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsferwawh.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhljorhb.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtvefqovy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvaubkzee.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gggtvajfk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/giridnkxu.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwcmpdsv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpfgtadx.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gdzgavqrm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsbgbpkfs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeyykeew.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkdjoav.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvblokap.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwrgczha.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdbkpais.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyjcbiun.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggidiregf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gxfrjpntv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmdqnuvt.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkhzirbag.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gctyvozpz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gyyxpxbsd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcovfzzy.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvbhcnemj.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkcnrcmla.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gwkuxaart.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/glcdyriyu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gyxtjqvmh.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvwnensa.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvwmjwow.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrwyywci.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gtnmdncki.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwxubweo.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gutbxnsxg.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwmvjlhs.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbehjgtmy.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gvpzjdfxw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuxqqshc.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvbzbithn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gelfejikj.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmixbjyx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geiwkuwcz.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gljjpnlxl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gsblqntoa.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumziaqym.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbhbgoxev.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gtezzlfek.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubhcwkbu.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpufbjqr.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosjqbsnd.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gnldiwtcx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdejtxgg.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsucgacgl.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtrgvrkt.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstufshnm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gufoeogvb.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhldfxmt.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgjhnuzq.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gbsrfyjmo.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gwoxknhua.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawtdxagd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gzfwszjnx.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/giukuwmph.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwkkvmcr.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtvzmzdcq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjytaeonq.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggiphtfvq.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gxeembjli.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnwygytwl.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhbocznc.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwmporaa.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjbhrcka.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuvdwcpf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgraxgtm.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gumtitpfu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfsqyhu.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqohnnzs.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gedpyhsem.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gcbbspdav.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhthhmux.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gqblcakey.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfirtydrj.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/geixkjttr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlphqxgr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcdovjpt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxkncqiv.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gpnfdjirf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/givhdeqbq.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ginxqgfpf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glctqqdwu.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/goxxqdqdd.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/govdwltjk.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjismnfd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyhixqqtr.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaordbbz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/goiyodmeu.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxfywzitz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gsjyzmypf.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gwfhebwyq.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gegczrgnk.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gmqpwqyov.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmhuhgtn.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gqecwoipf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbjlrpuqc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuxyvgit.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gtagqmrwz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixrjczvp.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuwfnytm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gblxajxth.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghhppyykp.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gierzlsix.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkzgibdt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpvydmmx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjbvrqya.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gxbyoetqf.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/ganyblgcg.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gcslnehcy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/galmehzzd.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvijrczj.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gsxwpqlhs.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfcagcpm.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfyxokza.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnsdmtzg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgcxizzs.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/guyosmxvp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixolmbma.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzcepuzn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gjjsemair.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuxmwkou.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/geyoamulw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyqineon.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkyfjtbf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcglpyads.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gkdkwetpk.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvxqwwvc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/grdmxbgsv.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gxujibtiz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gzavdfknu.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoaxvryg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gjlbzydfp.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuhuivbo.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gravlslew.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gzhcpfjzp.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnauqccbh.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuownkzo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpksbcwk.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzgmmbxj.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gscwohoxh.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gyhhikidp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gbamwmryw.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdgwrayl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmaptisr.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gulurmhfw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gtjadwndc.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gzlovaloq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/glhvyhpxl.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/girkdyvpz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgzbugdu.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/glslqvodu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gayhcmcnm.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbsditgs.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gagjkkixj.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gueakeldw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gaywjxyuw.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvufjpwc.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsryvvqv.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwpdahusm.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhpkvlfd.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtciabnyy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gvvcmebjf.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gernvzxlg.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpkbmpjk.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/getilycnd.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsesbnpis.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghftnwdrn.sHtML


<!-- 参考信息 -->