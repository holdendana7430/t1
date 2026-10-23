代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mkngwlqe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3guclzgjr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3axazeyqj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dpwqtszl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3akomlowr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lyyidask.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3eqqdsnnw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qhyfxyyc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dlrmnqia.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3frtgrabc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fpnyxpox.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lqmzwyzu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hhatvqok.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3sfrytccm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pnvujmlh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qdlupfcl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ojqrukgb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lryogeue.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ekrcchyt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qyltfmiw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rhrcsaxr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gcztepzo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dkbzqecf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3drgkblxz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3weysecsh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jdildwhy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fsvkpzyj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dgmamjuj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwtfkcpe.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hzagfuil.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bsofmttq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ihmovjkj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3odqqgajl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mazpbazh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vlasaqeh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ytdhyzhm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qjyyuepv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jbfrogvc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3stpnvvpy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bzhxuwsc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xbkdgwyp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zpzykqrw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ddobbjuu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3meqbqjjo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3gliakzcp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jswdtjvn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3irypequz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xyskwmrf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bisivtqd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjjgtcpr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qwdlgjal.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbihfdyp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qmpkqnew.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3viuuhkqx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3kbhxewru.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zfgcbgmm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zlvjtbcl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3eczoubaf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hquxtxht.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hzlkplfb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ikneukbx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3uquygtkd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3upialzyw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ynanlhux.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bbaghkuq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nkvnhphx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ialpytpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkjtwygn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gbmawhwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysadhpcm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tlbfajxe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nwaxwpio.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fxqvamil.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pxxklyop.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nuvwsfia.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ydbwjeor.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ymxkwffr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujobsitg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zaeymfrg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tdancljf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mjjgmxyh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hemcfyac.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3reocmeqc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cilgazas.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zkbmbtki.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qicseoxc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lhkrihro.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nakddnuv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wyntzqhd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tizqzebl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lgqdmvrc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vbdwqdgd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rhvngxrz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3izljdswu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kpujsgqg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3opzxjvxv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3maqemoyd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vhhmchbc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3onslodtk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3exjayfah.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lreaahjh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rgquxiog.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jqlfqsoj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iirfwfxh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mlfcstoj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3pbsqsxcw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vcdoltio.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yfxlzmvn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3brldvnyg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zwqdthzu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zmevnqtt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zfjepriw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3orfwxahk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3edvjgfxw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xtrdjytw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jetkkcag.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewjbzpug.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dxzxybmv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3wfvcabok.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ujhvpavc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jiaakixh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hdmolumr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3slofcabl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3zwzchudn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3opaeiuiy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3mpynjlhg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3idxkegme.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nysueqwz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rgjhbbhl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nwpvrjqw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cqiopzqy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fbsmndkz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vkaqwqwj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ayefzprj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hmalbwzz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wnhexhyy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3toopiiul.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uccplhhn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yrxbputx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3myesnhby.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ocmnfnsc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3tldllzyj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pmivpufk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vvyhlqgn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3smgoeypn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gzvoysfw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nbjhyvms.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ruqbdtrt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gzbuzfla.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3slonzedm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3nyvsamed.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3fsumdvoe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yblymtzl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hhvuhutq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vgknbomy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3mccsezhl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yadozvag.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nuircqdd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mhqqenjf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckxprrte.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zxjhdezm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3rxfxgfbj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cclwazyi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ezeewhqt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wvijkcma.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tpphpuuz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lcelylrq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3pqiixqaz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jgpsjtpi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zhixethc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jazorltm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3auyzgrdu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3lftilcew.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xvzazjvi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jrmeluph.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3yjmsezom.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3egpmwkdn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3xrdzgqhx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3omlqxosr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dggaewnu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qwwmyxrq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rbkzygai.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xwpdmaii.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jyneelvm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3whlugmrb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3thgjvtbm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dnswmhrv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jrikkxug.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kitupoak.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3upxsnhvl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3sftwsevv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mjxyzigp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qlzrzmox.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3apcixjky.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vtvknuas.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dvofuykj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ulbiwjyf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3owthhyzk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nrkkmdxj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3eqsvdwmn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3galnnhkd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3trgbpztl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ciyigslp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rraxdxhj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3etszmufa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ppngybyl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qbhwakmj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3meeuviqn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xoyxzokz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3llsudxhe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmjgdajv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qrpcbrlv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rlroprdp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3eavxogzc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rvxnyhjz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yahfcwux.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bekolbhc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lzmtgtxl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ccyvqtcg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wzzzxkmo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nkxbwdkh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ptsoulew.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3itaawamj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3iluflaqg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3guqbertm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3axauazqq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jirqohfs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3uksjfoua.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3umzgwfha.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kfvonklg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kxpcvbsj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jielyyra.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qhvqvpsv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3swsbadyc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jfllavsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ziobsfty.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3htryxory.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxbwlrdn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xoqxlgfu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kkqyzqtx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymmdtoyc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sklpgtvj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pjajemtc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ddbicfmp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3adnsryxu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rmggaxhm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iehmbkwt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lascahpl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuqyzoqp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lvosilqp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fiilxmmq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xfrxlmly.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rnjfznrn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3iapckecr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3sfbbrymq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mguumdvm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3kbwnptwu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hxqtwujp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qzidhdfm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rlyjmxkh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fasgymdf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dymkplrj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dbfoktxa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lvewmare.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mltnbsxl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ghsbttwx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kjzaoqny.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3zxbzkkde.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jhxnxebt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ndjyyfuf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3utlicegl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cshxzzkj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xspbdxyd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xmggqign.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lxhtjnuv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zvbbadng.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3isjytnlh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ocyzzbvb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qimbsufj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kymdyjio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ozlujmyv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3omyviryr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ipjzapem.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bthfyzzs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ohlbjzdv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3omhjckkb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tfmffvjq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tubkowta.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qaiwncos.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3eqjffzaz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jikloxvo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ftftjtbq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lhtamkuc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tbnyfdkc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aksssuxa.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qvtdpafb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3weoqviiy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3drqrthdf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jrntrtij.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3koaxzdju.html


<!-- 参考信息 -->