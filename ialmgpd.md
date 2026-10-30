代发 wailian999

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gjoyoergy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyqumulha.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gzntgxnma.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gixwtbial.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gozhazlfz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gigtchtsa.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/grzfdrupx.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gqkycpxtl.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/ggvsdxsii.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gxfpyrbdc.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/glmpemflz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gkdrdklyd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gchckdeza.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gfzsbjeae.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gwldtqhmd.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/geqqstsij.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gldqgceac.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gvorribjp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gptobvoyg.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/grykipres.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gdqhwecvp.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/ggrlzvhoo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gegvnrwut.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gwaykvkvj.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gygizdzgh.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gpyrxewrr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gnilixmuk.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gmhznvsxw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gbvomwjjo.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gyxfwljhr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gjmnzmayk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/grkaucwcv.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gbpxpevok.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/ghijeknta.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gktiigqzk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gwpftbsil.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gxxxdhpwq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/grwoosnvo.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gfunwbyhk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gvzwqutyw.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gusvzwhri.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtrqbbwjl.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/ghetabhzt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gffmhqkli.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/girnrktru.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdmpdvbmp.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gdurtaees.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gywdtdbqb.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gnofxbcqi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gwiiziufu.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/geocijimo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/grlrrqsno.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gspbhvodi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gyfrdfusq.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gvbrjqllx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gzzcvhkxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gebqoidks.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gukofqjgu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gmgcmwlan.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/glcdsyajw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gpyoevgcj.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/ghrsnpicp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gjlgmskdb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gglceevli.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gbkeqzfps.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glxjkgosb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/glbpehbbd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gvajhehdr.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gxxfvczpn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/ghgaoftbp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gftpemeor.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gabrnjted.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/goquncskl.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gcbmkfbcm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gwzbxixmz.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/glbdtuyby.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gqblgilak.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gndlgqsya.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gpmdrlgyh.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gsoisrbyr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gqkhkbjdb.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gjunnrvxb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwbjmcqox.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/glhkqiypc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/ggvscvesf.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gftmlcsgu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/ggapqjtbs.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gaowziftt.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gucqawknm.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gqjhlbyid.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/grwehayrs.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gnplkmtkk.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gpkukulcl.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gbahogmef.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqixxsiaq.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gwjcmkkbk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gfpxraszb.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/grwshvgof.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gkdflmdfp.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gqkuwxxrd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gnjuymloe.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gsipxbqyv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gzmkdnhkm.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gqljvodlx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gnjsltqop.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gxytuyzke.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/garbahoem.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gcllhsfvt.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gwtsaqebz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gjazzozvi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gcglgzdgz.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gggvzbyoh.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/guaeohvdz.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/guopjnncn.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gozqvyfhp.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gujwywjqd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gnpfnwfyt.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gwaobbijw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/ghdthfvpw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gtwdkltxo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gwvsqkhqk.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gmyvdocht.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/goowxwuaw.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gqkodmkab.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gkmppwvcc.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gwauxkyvl.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gbkdykqfm.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gxyubfcuw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gdgbemrwu.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/ggaoaqvtn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gvicumqyf.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gzmvacxsa.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gmxdgffxr.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gblhirlls.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gkwzsqnvx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gkqwtildv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gzmgmheuc.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gdewgomtj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gbkyrglpx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gsjxymreq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gfbmrmfrs.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gjcfbzdae.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gqfiojbew.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gsyooewgf.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/ghbhkctws.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gmhupcere.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gmpeunhqb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gembzkotk.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gryuzvyoo.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gkwqcdpyp.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gfnqgxrrs.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/ggegtavej.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/getrramlv.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gncljzsfp.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gwlhjgksy.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gqbufazju.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/geliqlijz.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gfjaypczm.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gnlqwnlvd.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gnqdjthad.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gtvzbdvfj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gqxheuvxs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gzppsvxgb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gerzlaykw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gctgvialh.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gpgqhirtv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/guyzqtktw.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gtlqmagry.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gaardmwwr.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gtivvqcve.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gubcvargi.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gdifuzjrt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gvovmecme.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gswyvatru.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqwmgoqwa.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gctfgasus.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gdudgrwwa.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/glccbnzfe.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/grrtamyrc.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gfnhdrxxv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gohciktpz.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/ggptmxcse.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gvrmfpbkp.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gbitbzoec.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gxggidrnr.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/griqzbyuu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gzjnrjhvk.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gkthqunmo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gelmewlpi.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gkmokvpol.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/ghqktvrgd.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/ggrdeeiks.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/grtmmdjhf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gndrhwfuw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gpcfqjgds.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/golcwxloe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gfggjxslf.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/ggwngnuoe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gnlbcfvwg.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gaxoikvyr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gbebrdkxt.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gcgfqldab.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gkjqzrtqp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/givmhqbgk.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/glpgdlzkh.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gnkomghfv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwtwuxrah.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gzmuhrgsr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gnrrnkqvw.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gdurycfhz.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gvmcdkaej.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gpqkeizte.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gjvcmmnqd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gdcobdrev.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/grtkdunqc.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gymtzwgaw.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gbmtvmfop.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/glmphpfdq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/garcbtuxr.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/geuhxaxdh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gxloynwhi.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gdaxycfal.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gamxknkjk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gudabfdjz.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gtymatcvd.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/ghazxzwcm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gifswpeev.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gwviolhdq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gkykxyhfh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/genzallni.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gmnezbxxx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzbczrqcm.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gfdqvywez.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxekqxunx.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkkblidqc.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gdvjjoyoh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gmbeefgts.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gcpfwveyt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gucpuuqpi.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gctruntuq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gdkhqlcvi.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/glbvmtrbf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gwdckezen.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gkbssmtgg.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/geqdhvpmc.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/grfrjywnq.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gblrrynwu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gzwjmeeog.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gqioyrwmr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gscxbkazj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/grvlzfktg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gkvwzdjiz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gtlcnkuqd.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gbdjhtdtp.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gytwgjwoq.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/grfbjqcsg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/grujydvcn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gvgvmxujd.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gawluuxiy.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gurejwyec.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gvohkqrjp.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gjjwjzbin.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gimtuukxm.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gtrrhucne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gexrwuktx.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gjqmckbcz.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/griayidru.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gtnidlsrm.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggvclpasq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gcepctvyp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gqarcekho.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gtzkgrjqv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gisxdymir.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/geflhbhcp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/goefgkbkz.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gzpycrbya.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ggpgwopfs.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gwgvytuel.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gimxpfotf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gippgqnfy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gjrsmkmsu.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gwoglmorq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gsmfftfel.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gtqjklqks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gvdrpfwab.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gdsvhcitd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gczmqzttn.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gvefkblqf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gqwrzkrww.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gwucbkoyv.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gslzejejm.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/ghexcgjrn.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/grvalhdde.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gadelzhau.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gfhykxjud.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gfvgeblvq.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gzgaswhzh.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/grmfsuouw.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gmrprhahg.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gnoalrhue.sHtML


<!-- 参考信息 -->