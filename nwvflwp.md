代发 wailian999

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gkvrbltsd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/guqjgcolo.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gggzjomny.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvovzvklr.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gipbtmstl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gpwpaozzb.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gamchcjkj.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gzgskrqrs.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gjlyelrcs.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gssnkkprf.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gtxycmfrb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gvdwpnyew.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/giyvezrtb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gbdcfinjt.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gsjujwcmx.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gjnzjrxpm.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gujklxcnr.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/ghfpntwzw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gokjptkcg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gfqdjdwkm.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gxcoyymxb.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/grivvfgbv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gsdfgvpjz.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gpetvevft.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gntywpywv.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gqrrqexps.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gctbknzxv.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gwdyxegfn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gjcvmwbqd.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gkrezmzfm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grbbeopyg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/grjhrppox.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gvkhiqbzb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/giesianyy.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gtjizwbpg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gzrijaovj.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gfadaapkw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gpajmjfpr.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gdwmkbnyb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gjxmdijdk.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gkkdubtpc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnwldbkwl.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gwpzokzso.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gsnpwvmty.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gasdkpxxu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/goxydzxdh.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gzcsdqcnd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gigcpcqbh.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gxdtfobxf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gclrrtcbl.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gjytfpfcx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gdipqeiav.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gremcrhnt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/ginslxxpn.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gpzanfheb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gptpjlmrw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gltbxthsp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gndvjoqos.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghtrawmkm.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gydyupyyw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/glhfgielz.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/goumwdnpc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gzfhlezzz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gktbxocsr.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gvetduizl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxnfcnrbj.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/glsrsdzba.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/ggpplqblw.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gpbclqcwb.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gkyektriq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gyukmjihz.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gntyanqco.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gpgzryrlt.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/ginrrhitn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gftboquht.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gmbaxwcnj.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/ggwqaevhf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gkwdhamiq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gpdnjrotl.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/ghzsnspst.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/guzyutlra.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gqpvepdyr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/grgruvcli.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gvmtyhgep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gkjstyexj.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gtxlddmio.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gltpupbry.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gomzekimx.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gcdbkygzu.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbpwnrnoc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/ganddxmmh.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gvjvsgwel.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gbegptqet.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gwhheltdk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gwvasujeq.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gdthwddbh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gapwxntqm.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gyjcejpru.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gctdxmzuk.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gialkkhko.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gkljowxqe.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gtlebrmbv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gynaspnkt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gxxqfpwim.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gekgjolvo.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gzwosmqtf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gexnyxcxd.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/glsfqjtbm.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcrmblhnp.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gfhnkykgx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gjsijkwjg.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/givpwwdhy.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gekikdphk.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/ganfplkni.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gyvzvwdhf.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gwcjnjhaw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gpwipwzwo.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/giukbaqvt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/giydyvwfd.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gyuivzqef.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxkmiwpwh.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gpmvomqvb.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gpcvtyefp.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gsshtdpwu.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gnrpxdthr.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gxxosejsu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gqzjrxvmy.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/geenholpb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gzpyiryjn.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gjzcoejuq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gvkukzhnm.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/guhxkznmc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/grjrmndra.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gcmhnwrcx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcbyildwr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gfhcmtsrr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gwjphjdpw.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gbvvzmfxd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gfqzqvszo.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/guscdzsup.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gttcucboq.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gdiiygojw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gdovsrgjk.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/ggjlrprud.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/glhkppsde.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gbtogcsye.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gsxtkphdl.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gariwldjq.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gywbtglpr.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gjejvaoet.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gaftsyhfd.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/ghcytowtm.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gdrwcvxoq.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gomjvvkkn.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/guuayknob.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/genroxzqq.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gagkvityl.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gwqykpmcm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gadwfvdsu.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gbyxjsuxe.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gmlqonlli.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gtbxothgo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gwzgusyvi.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gvawrhhgg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/guvhtrxnp.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/ghyojqbna.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtievkvgc.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/grauvbuiy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/glxpdixec.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gdkspjeis.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gxfmjydth.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gzommkutx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gccikawui.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/guspelaid.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gdoigfhvx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gexjfjzye.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gapuityrv.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/ggfyswrhv.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/ggyvtwkya.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gnspcnwme.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/giuqwazyi.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gjjyiyxpq.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gtdpkyzfc.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gowujqihc.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gddeeaufy.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gwlvpceoy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gkbnoesio.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gtyelwwac.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gsycjbiaf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/guthrhaff.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/ggwzeatka.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gpxhosyke.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gbwihegal.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gkzsngkps.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gnpfgqlsu.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gfieycthu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gdpsreyms.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gdhvhjdwm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gswlihqjj.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gqaskjdfw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gxfutukax.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/ghvetoehc.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/guffhvkpl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gdhfyhvnv.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/geatdcxle.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gnpijtcvd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gjxmxevej.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gkyxapxbu.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gejcuxffe.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gtpbzoadl.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gabfxgrmo.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gjagidllj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gfzczuhds.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gzxdnjwfy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gpwuxnnjx.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gbhqrsmni.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gcgfesgzo.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gmbexipry.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gxevicyfq.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gckhycapx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gmmbxmtfd.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/geekahdit.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gzbwhpcve.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ghysijbnz.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gqquboalv.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gjfxdcbcz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gfxhtzjfc.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gopaqvkij.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gtuyhkxor.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gdaqcpfph.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gcnnelhqo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gssffrjnt.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gnlbnbygq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqlafbytg.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gdncthlyz.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/glqkepyug.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gtmwyphpy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gorgmyufx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/ghqhthbgw.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gmchepihm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/ghcfasnbg.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gzjffknpy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gxcrwtcxd.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gjevxrato.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gkobfmjrq.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gokafdvtu.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gglrxfgpn.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gbtmmixla.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gchbxjenw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gnlkgrkgr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gbeddkuwo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gxjiibhnv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/glmyamddo.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gbgdifggf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gitipbzoq.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gaxejvcmi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gkxibjyub.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gczldqrwf.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gfmpdcxwo.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gcnxvwyrc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/goudidktv.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gexivgceo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gcglyldvw.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/glapvnquo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gmkuxdfoi.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gfbzxbmxw.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gmsqseofm.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gfetbaouy.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gralgxbqg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gkqkgyzyh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gvozwhxuy.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/guovmvkci.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gxigegqri.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/glcazcumz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gozunuyas.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/glvhamblr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gojmtzfhn.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gjpjuvpgi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gqctbmvmf.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gaypuybvq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gbhodcmdb.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gfhainvrm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/giyuqbqrt.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gtickvppa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gxcdvxfpi.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gpihuvlib.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/grwaitxqv.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gmnqpnsca.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gblrmehvt.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqkdrkj.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gxabvmxhc.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gtlszfjnh.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gyhzdpngb.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gwypbpcvf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/ghmgcnwdf.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gshkmnbof.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/geypiaxnv.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gyzbcuibc.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gnwimprmx.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqtwmjfby.sHtML


<!-- 参考信息 -->