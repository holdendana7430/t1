代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhaomingkeji.xyz/gtgcdophff.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtptbmxhoi.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangtech.top/gtburcajcn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenjidiqi.icu/gtvxjoryqw.html

[Q48] CTE 公用表表达式
来源：http://hz.guowangkeji.top/gtyjpcdfdy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nwbrower.top/gtqvjrubhp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtkdbjoclk.html

[Q49] 更新单行
来源：http://hz.fzhhl.top/gtupnnrsrl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtyjavlqli.html

[Q50] 批量更新
来源：http://hz.birdmap.top/gtnndysinp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xingfuxueyuan.xyz/gtkgvqkcsz.html

[Q51] 用子查询更新
来源：http://hz.ydjk.org.cn/gttlsswizj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gzhubu.top/gtauuymtqd.html

[Q52] 删除指定行
来源：http://hz.jyoumei.cn/gtkyfvwjzy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dashuyun.cn/gtgxwfwnba.html

[Q53] 按条件删除
来源：http://hz.zhixingplan.top/gtlhjxtege.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ybcxt.top/gtpeerzhzw.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gthnwqgjbm.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtfvwliphz.html

[Q55] 排名（并列占位）
来源：http://hz.guowangkeji.top/gtotypihxz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pycfn.com/gtixjpwwfd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhiwuduotai.top/gtdypjvfit.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daxiang520.top/gtymbzylxv.html

[Q57] 行号
来源：http://hz.nanxuanxn.top/gttrfvjjnq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhiwuduotai.top/gtjiqdabkh.html

[Q58] 累计求和
来源：http://hz.ydzc1.top/gtgcwclrhs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hammf.cn/gtnbfnixwd.html

[Q59] 分组内累计
来源：http://hz.snrcjt.cn/gtcqucswjo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhoulong.xyz/gtqxmkgquf.html

[Q60] 取上一行 / 下一行
来源：http://hz.xylfe.cn/gtopefzqdu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtvzmohkmx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.feifeiyinyue.top/gtmfklscgl.html

[Q61] 移动平均
来源：http://hz.guowangkeji.top/gtaxlxvkwf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj202588.top/gtttvlcgtu.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtipvifhyy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtcxmhnzod.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gtpjqebmbj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangkeji.top/gtrtlizkor.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtcauzwnef.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtmoddliom.html

[Q65] 回滚事务
来源：http://hz.smart0.xyz/gtutdlfvro.html

ROLLBACK;
来源：http://hz.yongpay.top/gtxgkwuxlo.html

[Q66] 行锁查询
来源：http://hz.tianlin.xyz/gtaristwbl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sxryk.cn/gtfdwrktlo.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtesjbyaxb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhijiandao.cn/gtngphovhf.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gthrzrkqpf.html

SAVEPOINT sp1;
来源：http://hz.gzhubu.top/gthrgknhvk.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gtldoxatrb.html

[Q69] 查看执行计划
来源：http://hz.yj20258888.top/gtenfgtpqj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gthqqxwhbi.html

[Q70] 更新统计信息
来源：http://hz.meibo888.top/gtdeprplfn.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtmfocuvli.html

[Q71] 查看建表语句
来源：http://hz.jiagoushi.top/gtxvtfyape.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtqkuyzryn.html

[Q72] 查看索引
来源：http://hz.aizwys.cn/gtfkvlxxgy.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtwlfjvgch.html

[Q73] 查看表状态
来源：http://hz.ydjk.org.cn/gtlqsxthmk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhixingplan.top/gtscbqalbx.html

[Q74] 强制使用索引
来源：http://hz.haohaochexian.top/gtwyhqkfoo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.havefunace.top/gtgypunpna.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtflhsaour.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtxxscimdg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hfpthk.cn/gtkgyopyea.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtlqkunfyo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xingfuxueyuan.xyz/gtlgpcpnbl.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtxtjkfqev.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fzhhl.top/gtlkhoycai.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gtpkjgvlbg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gttmrcixel.html

[Q79] 字符串拼接
来源：http://hz.hysaishi.cn/gtfyqjmxix.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigfzy.top/gtxpctgxzj.html

[Q80] 字符串截取
来源：http://hz.sweek.top/gtywvfpoly.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cqqwz.cn/gtytnrjftf.html

[Q81] 字符串替换
来源：http://hz.jinqigfzy.top/gtucufwtbo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtuwxdvequ.html

[Q82] 字符长度与字节长度
来源：http://hz.shuidangran.top/gtboezuxfx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258888.top/gtqlqptwaf.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtqnleqwqa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gthuugzmtt.html

[Q84] 去除首尾空格
来源：http://hz.cheryme.top/gttwquzldc.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtewjktuam.html

[Q85] 数值取整
来源：http://hz.jinghuilouyu.cn/gtoimrgeso.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhongyouzk.top/gtrmzghrps.html

[Q86] 读取 JSON 字段
来源：http://hz.vqdsnc.cn/gtozojusac.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gtfpgdcasf.html

[Q87] JSON 字段做条件
来源：http://hz.chenlongwang.top/gtmqoklzvy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gteuwszlmo.html

[Q88] 行转列（条件聚合）
来源：http://hz.shzxlz.cn/gtmckofaxa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.kuanghao11.cn/gtcztclleh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtbuahtjoi.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gtcdutmzhp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hfpthk.cn/gtiqhnfesw.html

[Q90] 生成序号列
来源：http://hz.meibo888.top/gtupwfyiqo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gzhubu.top/gtphhxtoed.html

================================================================================
来源：http://hz.quarkkingdee.top/gtfabjxvai.html

R. Bash 专题
来源：http://hz.jianghu66.top/gtnuzgsgel.html

================================================================================
来源：http://hz.daria6918.cn/gtndljwdpj.html

[R01] shebang 与严格模式
来源：http://hz.jqgfzy.top/gtujvvunrg.html

#!/usr/bin/env bash
来源：http://hz.sxryk.cn/gtxcywfyzu.html

set -euo pipefail
来源：http://hz.aizwys.cn/gtggotikjk.html

[R02] 变量赋值与使用
来源：http://hz.hammf.cn/gtzwrynvda.html

name="Tom"; echo "$name"
来源：http://hz.redwolf501.top/gtuzjhrbsf.html

[R03] 只读变量
来源：http://hz.yj202588.top/gtpxvrzgyk.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtfbumwjvj.html

[R04] 位置参数
来源：http://hz.ybcxt.top/gtkusfjpea.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenjidiqi.icu/gtcbukhsjj.html

[R05] 参数默认值
来源：http://hz.zhengqikj.top/gtuiwuaves.html

name="${1:-default}"
来源：http://hz.redwolf501.top/gtggcrrbco.html

[R06] 判断命令是否存在
来源：http://hz.hfpthk.cn/gtdnqmiofb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gaohongyu789.top/gtvgttbaub.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtktyvabuc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gtieullold.html

[R08] 数值比较
来源：http://hz.jqgfzy.top/gtuyocbvlf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtahqmelhf.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtjxxngdaz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtorudeaod.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gtojanmous.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhixingplan.top/gtbhmrygwd.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtepnhfsqf.html

case "$1" in
来源：http://hz.yuanzhike.top/gtyajyawef.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gtwvcywrbe.html

stop)  echo "停止" ;;
来源：http://hz.quarkkingdee.top/gtscbneqnk.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtnqdohxbb.html

esac
来源：http://hz.kuanghao11.cn/gtykwzibym.html

[R12] for 遍历文件
来源：http://hz.yj20258.top/gtiffeojze.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtdyttglvb.html

[R13] for 计数循环
来源：http://hz.52xcode.cn/gtberzqukj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtsogwnkvc.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gtgaqpxroc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tianlin.xyz/gtlrggwgaq.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtbuzaelpy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xinyue.icu/gtrspddypc.html

[R16] until 等待条件
来源：http://hz.guannengcc.top/gtelvkpmqb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtqspvojgg.html

[R17] 数组定义与取值
来源：http://hz.gogol.net.cn/gtsshlelcz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yanxiufei.cn/gtgilyqsut.html

[R18] 遍历数组
来源：http://hz.nwbrower.top/gtturkyzdf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gtlxpdntfj.html

[R19] 数组长度
来源：http://hz.fzhhl.top/gtktanvkxf.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gtcbforpgy.html

[R20] 关联数组（字典）
来源：http://hz.snrcjt.cn/gtxbxlhupm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cucudq.cn/gtnbhhpqhj.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtwrjbzuht.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtmwbkjwst.html

[R22] 截取子串
来源：http://hz.fengsongda.top/gtvrvpwfjm.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtydhkouum.html

[R23] 字符串替换
来源：http://hz.fengsongda.top/gthzhqjuue.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenjidiqi.icu/gtsrflrpgs.html

[R24] 大小写转换
来源：http://hz.cdnleiting.top/gtpkubdbic.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gttqacjufo.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangdashe.top/gteooarqlx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yonumen.top/gtqvknndak.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gtpkvijlcm.html

now=$(date +%F); echo "$now"
来源：http://hz.yuanzhike.top/gtadxldnxe.html

[R27] 算术展开
来源：http://hz.fengsongda.top/gtxlyjtvjt.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtlvyhcugu.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtvmrronem.html

echo "scale=2; 10/3" | bc
来源：http://hz.yonumen.top/gtiylmasku.html

[R29] 定义函数
来源：http://hz.chenlongwang.top/gtazyfmhtr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.birdmap.top/gthmzlxilb.html

[R30] 函数返回状态码
来源：http://hz.pycfn.com/gtlyvnjpll.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtbinosade.html

[R31] 局部变量
来源：http://hz.cqqwz.cn/gtbicaepsn.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtaheovgyi.html

[R32] 参数个数校验
来源：http://hz.shzxlz.cn/gtxzoqcsun.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sysykeji.top/gtxoqqdzxp.html

[R33] 捕获错误并提示行号
来源：http://hz.meibo888.top/gtdcwmwmim.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtivluxuga.html

[R34] 退出时清理
来源：http://hz.aizwys.cn/gtccmyxgyz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtxviyomqs.html

[R35] 后台执行并等待
来源：http://hz.yueranfly.top/gtnofbgrsz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yongpay.top/gtqbtwkawh.html

[R36] 并发执行多个任务
来源：http://hz.hnxiangtu.top/gtmszawqbd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinyuanbaomall.cn/gtzpeymgbi.html

[R37] 把输出赋给变量
来源：http://hz.yuxming.cn/gtgcxzlgkf.html

files=$(ls -1)
来源：http://hz.zhaomingkeji.xyz/gtefjnwjdi.html

[R38] 管道串联
来源：http://hz.sxryk.cn/gtnkkgcueh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnxiangtu.top/gtgxpeiwaa.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtrkpwojbm.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtrpzcudmb.html

[R40] 追加写日志
来源：http://hz.sweek.top/gtvnabzukm.html

echo "log" >> out.log
来源：http://hz.c1oappe.top/gtzmvamiuw.html

[R41] 丢弃输出
来源：http://hz.pycfn.com/gttlyxhqtr.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtpdodmvtf.html

[R42] 输入重定向
来源：http://hz.yvedp.cn/gtfcqzbcfw.html

wc -l < a.txt
来源：http://hz.birdmap.top/gtqwukdlct.html

[R43] 按名字查找文件
来源：http://hz.redwolf501.top/gtmjvucvqx.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtildsllhp.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gttceqibzl.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtfmriwdur.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtfzwvumjr.html

find . -name "*.tmp" -delete
来源：http://hz.jqgfzy.top/gtzytyvavz.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtouqrwycd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuxming.cn/gtkauyjznd.html

[R47] sed 单行替换
来源：http://hz.jqgufenzy.top/gtxiweavdx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yueranfly.top/gthviukrfn.html

[R48] awk 取指定列
来源：http://hz.jinqigufen.top/gtetbjnvtj.html

awk '{print $1, $3}' a.txt
来源：http://hz.c1oappe.top/gthilsunag.html

[R49] awk 带条件
来源：http://hz.hfpthk.cn/gtygzlzaiv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gaohongyu789.top/gtrgjdibmi.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtjlzauusf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenlongwang.top/gtfbzgeyrp.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gtlqprbhku.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxinkj.top/gtscruzpqh.html

[R52] 统计行数
来源：http://hz.mhx1999.top/gthfjeuxbw.html

wc -l a.txt
来源：http://hz.dianchejie.cn/gtnwycdpzn.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtfsksxucb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtprcdjtzq.html

[R54] 比较两个文件
来源：http://hz.shuidangran.top/gtwkqldhdc.html

diff a.txt b.txt
来源：http://hz.xuanzx.com/gtndmkqhma.html

[R55] 压缩与解压
来源：http://hz.tianlin.xyz/gtexubntla.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigufen.top/gtiutvopdf.html

[R56] 远程拷贝
来源：http://hz.ydjk.org.cn/gtracshojx.html

scp file user@host:/path/
来源：http://hz.0kj1m.cn/gtyyymbzov.html

[R57] 远程执行命令
来源：http://hz.zhaomingkeji.xyz/gtplnxdlmr.html

ssh user@host 'uptime'
来源：http://hz.yongpay.top/gtiqdwlgmw.html

[R58] 下载文件
来源：http://hz.kuanghao11.cn/gtzwqdzfcy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cheryme.top/gtlqzqvwwi.html

[R59] 发 POST JSON
来源：http://hz.vqdsnc.cn/gtkyjcxqib.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.kuanghao11.cn/gtqzmcpizw.html

[R60] 只看 HTTP 状态码
来源：http://hz.sysykeji.top/gtmanjwmqr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tian-w.cn/gtkuvekavb.html

[R61] 磁盘占用
来源：http://hz.yonumen.top/gtwfbixqiy.html

df -h;  du -sh *
来源：http://hz.feifeiyinyue.top/gtixiyziav.html

[R62] 找最占空间的文件
来源：http://hz.gzhubu.top/gtmchxusgi.html

du -ah . | sort -rh | head -10
来源：http://hz.shzxlz.cn/gtaxuwcuhz.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gthslkonig.html

free -h;  ps aux | grep nginx
来源：http://hz.xuanzx.com/gtccrpnbrg.html

[R64] 结束进程
来源：http://hz.redwolf501.top/gtwjwrsdno.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtldsjoolx.html

[R65] 查看端口占用
来源：http://hz.jinyuanbaomall.cn/gtlmaqgjpe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtfvwpkmaa.html

[R66] 定时任务
来源：http://hz.tianlin.xyz/gtlbiznnrm.html

crontab -e;  crontab -l
来源：http://hz.guannengcc.top/gtbieoztdr.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtoxnvcwjm.html

openssl rand -hex 16
来源：http://hz.chenzaomai.com/gtbaizwndi.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtlrxwmumf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxinkj.top/gtlekycpun.html

[R69] 生成随机密码
来源：http://hz.cheryme.top/gtmuscykne.html

head -c 16 /dev/urandom | base64
来源：http://hz.aizwys.cn/gtmomeuavv.html

[R70] 时间戳与互转
来源：http://hz.quarkkingdee.top/gtbfxrpknb.html

date +%s;  date -d @1700000000
来源：http://hz.hnqzz.top/gteseppwim.html

[R71] 日期格式化
来源：http://hz.daxiang520.top/gtpawalrhq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tianlin.xyz/gtzzgbqfkd.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangtech.top/gtfyjtvjrr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cqqwz.cn/gtvkahgnbf.html

[R73] 分割大日志
来源：http://hz.yuxming.cn/gtchqmlfjn.html

split -l 1000 big.log part_
来源：http://hz.ivvv.top/gtreerkqdp.html

[R74] 批量重命名
来源：http://hz.hammf.cn/gtyzosronu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258.top/gtcmxvxvss.html

[R75] 导出环境变量
来源：http://hz.yuxming.cn/gtqgleglxv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gtksfzuinv.html

[R76] 使用临时文件
来源：http://hz.hywenlv.cn/gtseptsuyx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtyafulthf.html

[R77] 读取用户输入
来源：http://hz.ywan-chungtsiang.top/gttqellvni.html

read -rp "请输入: " ans
来源：http://hz.zhaomingkeji.xyz/gtdurgoypo.html

[R78] 交互式菜单
来源：http://hz.svipenyu.cn/gtvnsbftqi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jlsjyb.cn/gtfapjrbal.html

[R79] 解析命令行选项
来源：http://hz.c1oappe.top/gtthzwyoxl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sxryk.cn/gtpoefqzbf.html

[R80] 查看脚本执行耗时
来源：http://hz.cashguo.top/gtehqbbrva.html

time ./run.sh
来源：http://hz.yj20258.top/gtqutriotr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtaxyyknhy.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtafdjiwsm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtkhtrpyqy.html

[S01] C：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtadgasxtb.html

#include <stdio.h>
来源：http://hz.kuanghao11.cn/gtwytkkloz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.quarkkingdee.top/gtpxzwyeil.html

[S02] C：变量与格式化输出
来源：http://hz.yanxiufei.cn/gtqfrzgfqp.html

int a = 10; printf("%d\n", a);
来源：http://hz.yvedp.cn/gtuxsyxdpl.html

[S03] C：读入整数
来源：http://hz.guowangkeji.top/gtucifoyjm.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtluavoqso.html

[S04] C：字符串复制
来源：http://hz.hywenlv.cn/gtgrlsakzw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gtcyhmwjjf.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gtrcqznxkg.html

strlen(s)
来源：http://hz.ydzc1.top/gtitynbvzw.html

[S06] C：字符串比较
来源：http://hz.ydjk.org.cn/gtpumllsye.html

strcmp(a, b) == 0
来源：http://hz.xinyue.icu/gtnzughmip.html

[S07] C：数组遍历求和
来源：http://hz.gzhubu.top/gtefomvfda.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guowangkeji.top/gtxxkhnwou.html

[S08] C：动态内存分配与释放
来源：http://hz.quarkkingdee.top/gtwdsvhbdp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hysaishi.cn/gtivmnjgmb.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gtgtcvvqsc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtdillbzrk.html

[S10] C：指针与解引用
来源：http://hz.xuetiantiany.cn/gtryyeqvms.html

int *p = &a;  *p = 5;
来源：http://hz.hammf.cn/gtdkvdxoco.html

[S11] C：逐行读文件
来源：http://hz.hfpthk.cn/gttdmxyvsd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.316326.xyz/gticqtmpjs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.iojbl.cn/gtngaevwpg.html

fclose(f);
来源：http://hz.sysykeji.top/gtpkfviler.html

[S12] C：写文件
来源：http://hz.sxryk.cn/gtdfbozsel.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.bjfxy.top/gtunasegcl.html

[S13] C：宏定义
来源：http://hz.zhongyouzk.top/gtbmucjwcw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gtdehowtyi.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gthngjhzru.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtylganvmj.html

[S15] C：类型转换
来源：http://hz.andypj.xyz/gtskzrscjk.html

(double) a / b
来源：http://hz.yueranfly.top/gtollkblzg.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gthwvuoycl.html


<!-- 参考信息 -->