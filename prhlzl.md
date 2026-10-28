代发 wailian999

[Q44] IN 子查询
来源：http://hz.zdqjudy.top/gtrzoamdhn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hysaishi.cn/gtnxkvnckw.html

[Q45] EXISTS 判断存在
来源：http://hz.yuxming.cn/gtuazadfnt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtqsccougp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tanke756.top/gtxmosowys.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gtezygqljb.html

[Q47] 与平均值比较
来源：http://hz.c1oappe.top/gtnwdajcxm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangdashe.top/gtrvhgztmk.html

[Q48] CTE 公用表表达式
来源：http://hz.hammf.cn/gttptilvxj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tanke756.top/gtqisnzjrm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhaomingkeji.xyz/gttvupiewp.html

[Q49] 更新单行
来源：http://hz.xinyue.icu/gtqutvfokx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.meibo888.top/gthulajhcd.html

[Q50] 批量更新
来源：http://hz.sysykeji.top/gtvlxwlxek.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gtpnweniex.html

[Q51] 用子查询更新
来源：http://hz.zhengqikj.top/gtaogruyuk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydzc1.top/gtjxyfxoxn.html

[Q52] 删除指定行
来源：http://hz.hnxiangtu.top/gtfqsruggg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnqzz.top/gtjihijudv.html

[Q53] 按条件删除
来源：http://hz.aibaodan.cn/gtxrvmrpwl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj20258888.top/gtifdtnsci.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gticvcjddc.html

TRUNCATE TABLE logs;
来源：http://hz.daxiang520.top/gtfogfmvaw.html

[Q55] 排名（并列占位）
来源：http://hz.pycfn.com/gtneguoitu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhiwuduotai.top/gtymsepryb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigufen.top/gtnwpugxee.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ydjk.org.cn/gttqvjrtqw.html

[Q57] 行号
来源：http://hz.tian-w.cn/gtispgdkdf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinghuilouyu.cn/gtmdrjnmcr.html

[Q58] 累计求和
来源：http://hz.andypj.xyz/gttzufcjzl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.snrcjt.cn/gtqgdutejc.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtxzpwvonu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pycfn.com/gthwveonni.html

[Q60] 取上一行 / 下一行
来源：http://hz.nwbrower.top/gtlycxcabz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hysaishi.cn/gtpsopdvji.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dashuyun.cn/gtavzscomc.html

[Q61] 移动平均
来源：http://hz.sysykeji.top/gtpknztuox.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.haohaochexian.top/gtdbtjvgzn.html

[Q62] 分组占比
来源：http://hz.daxiang520.top/gtwfedyypd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtndqvgijh.html

[Q63] 开启事务
来源：http://hz.yonumen.top/gteumxdkbe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuanzhike.top/gtpoqfdroh.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gtxvcablpk.html

COMMIT;
来源：http://hz.yangfankeji.com/gtwhjydkgt.html

[Q65] 回滚事务
来源：http://hz.52xcode.cn/gtydfqnhuw.html

ROLLBACK;
来源：http://hz.gzhubu.top/gtobrqvmch.html

[Q66] 行锁查询
来源：http://hz.sweek.top/gtqrvhtscl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.vqdsnc.cn/gtjxcmkbpe.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gtyaihbmod.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhaomingkeji.xyz/gtnjsevbeq.html

[Q68] 保存点
来源：http://hz.quarkkingdee.top/gtxyjlvecp.html

SAVEPOINT sp1;
来源：http://hz.sufxvd.cn/gtfywgowlj.html

ROLLBACK TO sp1;
来源：http://hz.ywan-chungtsiang.top/gtrzhsnpcz.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gtpuutaicx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtwsmxpfmv.html

[Q70] 更新统计信息
来源：http://hz.havefunace.top/gtgsrfnqcf.html

ANALYZE TABLE users;
来源：http://hz.jinyuanbaomall.cn/gtlusestlk.html

[Q71] 查看建表语句
来源：http://hz.ppjwa.cn/gtgtrceicn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shanyushiyangtech.top/gtxaarthoe.html

[Q72] 查看索引
来源：http://hz.daxiang520.top/gtsitczaqc.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtiigzcewi.html

[Q73] 查看表状态
来源：http://hz.hysaishi.cn/gtqftqeimy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.9152youxi.cn/gtukewhkbg.html

[Q74] 强制使用索引
来源：http://hz.pengpengdd.cyou/gtlszordok.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtwrqneumw.html

[Q75] 日期格式化
来源：http://hz.xziqi.cn/gthbxqaxku.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuxming.cn/gtasjpbqos.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gtukuugmyd.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtkiynygow.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fzhhl.top/gtxxzqmxji.html

[Q77] 时间加减
来源：http://hz.gzhubu.top/gtckrhbwyi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258.top/gtwpccpjwg.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtdmjknxby.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yvedp.cn/gtaaxzkqvj.html

[Q79] 字符串拼接
来源：http://hz.zhixingplan.top/gtipxkaenp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.havefunace.top/gtxqbszagp.html

[Q80] 字符串截取
来源：http://hz.tian-w.cn/gtszvtmark.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigufen.top/gtvsubaofy.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtektzbkyi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.316326.xyz/gthvfplvgz.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gtwkaojxtl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtglrxqgdx.html

[Q83] 大小写转换
来源：http://hz.jinqigufen.top/gtbbqczpru.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtdoarvydq.html

[Q84] 去除首尾空格
来源：http://hz.kuanghao11.cn/gtgiqgmfdo.html

SELECT TRIM(name) FROM users;
来源：http://hz.ivvv.top/gtxgflienb.html

[Q85] 数值取整
来源：http://hz.sxryk.cn/gthqacjlqe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhaomingkeji.xyz/gtfytrfpuc.html

[Q86] 读取 JSON 字段
来源：http://hz.ehwqpu.com/gtmhnpnubc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daxiang520.top/gtaxdtlsmh.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gteezygqls.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ivvv.top/gteuqmgkza.html

[Q88] 行转列（条件聚合）
来源：http://hz.daria6918.cn/gthqufjfjw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtrknfttbh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtxdfcnotj.html

[Q89] 判断表是否存在
来源：http://hz.ppjwa.cn/gtankaiigq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ehwqpu.com/gtalacnmsq.html

[Q90] 生成序号列
来源：http://hz.zhaomingkeji.xyz/gtehcejbkw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yanxiufei.cn/gtdpzaxjnz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkhyctxum.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtfaovlfio.html

================================================================================
来源：http://hz.nanxinkj.top/gtnwpfczhe.html

[R01] shebang 与严格模式
来源：http://hz.haohaochexian.top/gtslaspcjm.html

#!/usr/bin/env bash
来源：http://hz.feifeiyinyue.top/gtayavmtlv.html

set -euo pipefail
来源：http://hz.vqdsnc.cn/gtjikxgebu.html

[R02] 变量赋值与使用
来源：http://hz.shzxlz.cn/gtyklkajug.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtiphsqcyb.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gtynrdhttx.html

readonly PI=3.14
来源：http://hz.yueranfly.top/gtvfkccfhs.html

[R04] 位置参数
来源：http://hz.shuidangran.top/gtrjaleqhp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gogol.net.cn/gtgukwevqs.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gtekkzbkug.html

name="${1:-default}"
来源：http://hz.gzhubu.top/gtezlyqeaj.html

[R06] 判断命令是否存在
来源：http://hz.cucudq.cn/gtsgyailqj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cucudq.cn/gtydjbufvb.html

[R07] if 判断文件
来源：http://hz.mhx1999.top/gtzgwzhaom.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aibaodan.cn/gtrvcjebxl.html

[R08] 数值比较
来源：http://hz.feifeiyinyue.top/gtmmicozap.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fzhhl.top/gtjqvbrldq.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gtgfvravbx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zdqjudy.top/gtetxhepnw.html

[R10] 正则匹配
来源：http://hz.fengsongda.top/gtcczsehvw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hongshengwenyu.top/gtqvjfuyzn.html

[R11] case 多分支
来源：http://hz.jqgfzy.top/gtbscceitp.html

case "$1" in
来源：http://hz.zhengqikj.top/gtxictzabj.html

start) echo "启动" ;;
来源：http://hz.zhongyouzk.top/gtdbvcaovo.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtyqzfijeh.html

*)     echo "未知命令" ;;
来源：http://hz.zycfv.cn/gtvcbqtjiw.html

esac
来源：http://hz.daria6918.cn/gtrwnsqchy.html

[R12] for 遍历文件
来源：http://hz.shangyingyoupin.top/gtnqqoixen.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhengqikj.top/gtnbvmtslx.html

[R13] for 计数循环
来源：http://hz.hammf.cn/gtugpfjrlr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtqhcihlgr.html

[R14] C 风格 for
来源：http://hz.aibaodan.cn/gtubglfefn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gtslaftyqb.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gtnaifvkzf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dianchejie.cn/gtleveyquy.html

[R16] until 等待条件
来源：http://hz.zhixingplan.top/gtmfunehmm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtsygptmjb.html

[R17] 数组定义与取值
来源：http://hz.dashuyun.cn/gtrtveexmc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xziqi.cn/gtietecjwn.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gthqtuhion.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhijiandao.cn/gtwatawham.html

[R19] 数组长度
来源：http://hz.ybcxt.top/gtxrpjshxt.html

echo "${#arr[@]}"
来源：http://hz.tianlin.xyz/gtjjfhcziv.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gthmjdoxwk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtwmohkydi.html

[R21] 字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtwdhatort.html

echo "${#s}"
来源：http://hz.yj20258.top/gtyueylgcf.html

[R22] 截取子串
来源：http://hz.haohaochexian.top/gtzyfdjfpp.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtinyzjqez.html

[R23] 字符串替换
来源：http://hz.sysykeji.top/gtrylnecdy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gtjbddkxmf.html

[R24] 大小写转换
来源：http://hz.yj202588.top/gtqzqdndvd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gotoacloud.top/gtuclfdtjh.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtjrpjtfxc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cheryme.top/gtzgobgjwg.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtjcnmscdl.html

now=$(date +%F); echo "$now"
来源：http://hz.sysykeji.top/gtcepepxlb.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gtldcfaqwu.html

echo $((1 + 2 * 3))
来源：http://hz.xziqi.cn/gttdnfgvcv.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gtsyicrrur.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuanzhike.top/gtrstvdkdf.html

[R29] 定义函数
来源：http://hz.aizwys.cn/gtarmvszqz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cashguo.top/gtwacoekcl.html

[R30] 函数返回状态码
来源：http://hz.hysaishi.cn/gtftxrftfm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gzhubu.top/gtjpiabisk.html

[R31] 局部变量
来源：http://hz.feifeiyinyue.top/gtifruqzzf.html

f() { local x=1; echo "$x"; }
来源：http://hz.xylfe.cn/gtjdpwqagl.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtwfyyvhhq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtloyyyuir.html

[R33] 捕获错误并提示行号
来源：http://hz.316326.xyz/gtjzxlwhej.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gtxjcqqebj.html

[R34] 退出时清理
来源：http://hz.zhiwuduotai.top/gtdaxjwhmr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtlckvugxv.html

[R35] 后台执行并等待
来源：http://hz.xziqi.cn/gtnzxhaktz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shuidangran.top/gtkungisyl.html

[R36] 并发执行多个任务
来源：http://hz.zdqjudy.top/gtzuvykxpb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fzhhl.top/gtdfnktjzm.html

[R37] 把输出赋给变量
来源：http://hz.xuetiantiany.cn/gtwaknebql.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtwyoaywyu.html

[R38] 管道串联
来源：http://hz.xylfe.cn/gtwyedwkoz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jiagoushi.top/gtntayuraj.html

[R39] 重定向标准输出与错误
来源：http://hz.wangdashe.top/gtfuquyees.html

cmd > out.log 2>&1
来源：http://hz.yanxiufei.cn/gtsuapprqh.html

[R40] 追加写日志
来源：http://hz.nwbrower.top/gtietntmgq.html

echo "log" >> out.log
来源：http://hz.sweek.top/gtsqoamvly.html

[R41] 丢弃输出
来源：http://hz.jianghu66.top/gtgqdgqslf.html

cmd >/dev/null 2>&1
来源：http://hz.ppjwa.cn/gthxpnydbs.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtoodesaop.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtesmtixdc.html

[R43] 按名字查找文件
来源：http://hz.jinqigfzy.top/gtnorklhll.html

find . -name "*.log" -type f
来源：http://hz.shangyingyoupin.top/gtdlupvoqn.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtywiqroit.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtjbtznxow.html

[R45] 批量删除
来源：http://hz.chenjidiqi.icu/gtdrrmotqi.html

find . -name "*.tmp" -delete
来源：http://hz.mhx1999.top/gtttqjwvkl.html

[R46] 递归替换文件内容
来源：http://hz.52xcode.cn/gtkkgdgatd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtgewhrjmw.html

[R47] sed 单行替换
来源：http://hz.jyoumei.cn/gtlgpxdqnt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxinkj.top/gtovbiwehz.html

[R48] awk 取指定列
来源：http://hz.andypj.xyz/gtpyvbufez.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgufenzy.top/gtyljwcatj.html

[R49] awk 带条件
来源：http://hz.shuidangran.top/gtjgvkixpj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxinkj.top/gtpvxkosva.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtxthqcbtj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtefeubysu.html

[R51] 排序去重取前几
来源：http://hz.ehwqpu.com/gtapmjbdoj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gtkervtjul.html

[R52] 统计行数
来源：http://hz.jinqigufen.top/gthnqmebqn.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtezjthcvm.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtoirqlqwq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daxiang520.top/gthzbhbknn.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtrgwhasua.html

diff a.txt b.txt
来源：http://hz.yj202588.top/gttnrdsowp.html

[R55] 压缩与解压
来源：http://hz.cqqwz.cn/gtjopgkscx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtqiiqlvsa.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtzdplbysi.html

scp file user@host:/path/
来源：http://hz.xingfuxueyuan.xyz/gtnmuvbpdp.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtduliokzl.html

ssh user@host 'uptime'
来源：http://hz.iojbl.cn/gtaznkbbeb.html

[R58] 下载文件
来源：http://hz.316326.xyz/gtcmrwgeka.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtvlkheyrv.html

[R59] 发 POST JSON
来源：http://hz.hammf.cn/gtvkufowsv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gtunkhhtcy.html

[R60] 只看 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtnkrxqked.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinghuilouyu.cn/gtgoqsjcwf.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtpungseba.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtunqappij.html

[R62] 找最占空间的文件
来源：http://hz.hywenlv.cn/gtljlizwds.html

du -ah . | sort -rh | head -10
来源：http://hz.tanke756.top/gtzyfkxkjj.html

[R63] 内存与进程
来源：http://hz.hnxiangtu.top/gtambsdntz.html

free -h;  ps aux | grep nginx
来源：http://hz.gogol.net.cn/gtwwahpamo.html

[R64] 结束进程
来源：http://hz.wangshuangyany.cn/gtxehpthfd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.bjfxy.top/gtjwhdoaop.html

[R65] 查看端口占用
来源：http://hz.yj20258.top/gtazknghva.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gttmkbmjxs.html

[R66] 定时任务
来源：http://hz.dianchejie.cn/gtihobqjel.html

crontab -e;  crontab -l
来源：http://hz.tanke756.top/gtocsqgbuf.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gtsebyfecn.html

openssl rand -hex 16
来源：http://hz.guannengcc.top/gthaozkklv.html

[R68] 计算文件校验值
来源：http://hz.havefunace.top/gtqojyrucg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gotoacloud.top/gtrxqsyays.html

[R69] 生成随机密码
来源：http://hz.tian-w.cn/gthjidvrgd.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gtuismyaja.html

[R70] 时间戳与互转
来源：http://hz.yanxiufei.cn/gtzgcazfwn.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigfzy.top/gtuigvpscy.html

[R71] 日期格式化
来源：http://hz.jianghu66.top/gtrxisucna.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.havefunace.top/gtooexqdhg.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gthtjvfype.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fzhhl.top/gtspjmgdfn.html

[R73] 分割大日志
来源：http://hz.shangyingyoupin.top/gttnxycqup.html

split -l 1000 big.log part_
来源：http://hz.cheryme.top/gtiniuyyhs.html

[R74] 批量重命名
来源：http://hz.quarkkingdee.top/gtllyevral.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.svipenyu.cn/gtaomsjlpo.html

[R75] 导出环境变量
来源：http://hz.zhixingplan.top/gtqmsulgwb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daxiang520.top/gtvvmjlwtf.html

[R76] 使用临时文件
来源：http://hz.sxryk.cn/gtujduizqc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtadaetrxj.html

[R77] 读取用户输入
来源：http://hz.shuidangran.top/gtdmvcmnge.html

read -rp "请输入: " ans
来源：http://hz.yueranfly.top/gtizbokopn.html

[R78] 交互式菜单
来源：http://hz.tian-w.cn/gtnzcmumrw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ivvv.top/gtfwwbwrfr.html

[R79] 解析命令行选项
来源：http://hz.ehwqpu.com/gtxyjjagea.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hongshengwenyu.top/gtdrgqlwex.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtwhaapmeb.html

time ./run.sh
来源：http://hz.yj20258888.top/gtvaltsity.html

================================================================================
来源：http://hz.ydjk.org.cn/gtlvkmdajd.html

S. C / C++ 专题
来源：http://hz.316326.xyz/gtjskdvfar.html

================================================================================
来源：http://hz.gotoacloud.top/gtzphwfyho.html

[S01] C：Hello World
来源：http://hz.jlsjyb.cn/gttgfghyrp.html

#include <stdio.h>
来源：http://hz.jinqigufen.top/gtqkndosvd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.9152youxi.cn/gttwoauopu.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtbkknltuw.html

int a = 10; printf("%d\n", a);
来源：http://hz.feifeiyinyue.top/gtcjnxnknw.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtnmabpfhd.html

int x; scanf("%d", &x);
来源：http://hz.c1oappe.top/gtqbafpwfo.html

[S04] C：字符串复制
来源：http://hz.yuanzhike.top/gtykksqenm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gtdtzicsrc.html

[S05] C：字符串长度
来源：http://hz.zhongyouzk.top/gtlfjswezh.html

strlen(s)
来源：http://hz.yj202588.top/gtatprbnhk.html

[S06] C：字符串比较
来源：http://hz.52xcode.cn/gtdkibhmzg.html

strcmp(a, b) == 0
来源：http://hz.haohaochexian.top/gtjrjkvrzu.html

[S07] C：数组遍历求和
来源：http://hz.jianghu66.top/gtmttbahhn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jlsjyb.cn/gtufhltmpu.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtduwshffx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuanzx.com/gtklmxpuvg.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gtfnxnqcgg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gtohsjywex.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtffhmqrlc.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gtswhbwyzv.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gtckehejjn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuanzhike.top/gtfoiismqf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.smart0.xyz/gtlutekkto.html

fclose(f);
来源：http://hz.chenzaomai.com/gtfykoupse.html

[S12] C：写文件
来源：http://hz.ehwqpu.com/gtrgvspwtb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhongyouzk.top/gtocoytpxa.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtstrzxmjr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtuupotrya.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gtxdcwosih.html


<!-- 参考信息 -->