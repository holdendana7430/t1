代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2oomxhuub.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pwyxzqtc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xyvpddoe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2yacljukf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pxaubydc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wjyblpdk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mdclbsdy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pdpqckwn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ceriaamh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2momfsswr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tgtmbrjt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kufssokj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nwpmsnlr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tktnypaa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mgnlphmx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gcbyzmup.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2thktggsi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mxeadhfy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ispnevzc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rmjzhoiz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2cywucfxg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2nhiyetqx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2miacqlwm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hybukbjo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rkgjceor.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2dqozhvio.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncvrsnzm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ojgexztq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vowuvzsl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2gmadvyxe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jghnqmrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufkxaloh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vvuriidb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vimzrjmq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2laoxzriu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2gfgxmdaq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lkkzgfjt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2sshiqvqn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nmiobluk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ibslantk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ansvpzit.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xiqaagzt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fbhhnntt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zylmtcii.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2sbiqgyri.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ppnprfpq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jllgqggl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2getzsdit.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2trcismru.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2sqdbslov.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pgblauet.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nertonqa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mdeixmae.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jkcbutyp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2brgxwkpw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jjoiienz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2hfcrdimd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xmjlcnpo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vurrqmiv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lzgsqehg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gdgcnxfh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2peualukd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nfjcuzgn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2taefimct.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mzmcvdxn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rfuzowiu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nmsrvipz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezenofhn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ebsxbmbp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2acivfnvy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ydfwkvwi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yqtnqttj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofyuvbzu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2luvpkjkw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tvkmjsam.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sbjmcnej.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ejhifoht.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2cxvejirc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ajkewsuk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gcrvqqal.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2cezpbdhn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vzctzjnc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ychbimup.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2znpzuzqa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2aemaqafr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2umqtjbah.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rzersjjj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wtrmilnl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ugyclecn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2pmaftizc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mckjgqeb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xlavyqfm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qiiltssq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tbinfrtg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2usfajqrn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bqrkghmz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gotfhaew.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ztevvrbi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xlzjnsxt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fdfiwesb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2sjpvqtfg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2azxqeojp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmizpgit.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2sibqrqoh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zlpyyucs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2yodedcvk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qeqrbjou.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2emtjngoy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ehqptsan.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tbkxnbiw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qcibjxbs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uawozohw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hloixsms.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cyzekzhr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wtksbelc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gdayqhsb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2krmrkxjw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bifegofh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2duhpherp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bthmxiwj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bnmivdsw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ujtioqnv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2blpvqgii.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvyqqggj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2goydhtlr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2eqorzuuh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cqwhpsev.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2uyeahrsj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2arrxvcqx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fhizznex.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ltkcsdvw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bwbshfrk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hhxypunb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pkpvzkmh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zlysuzfz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dfleaaaa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ieejdqef.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xlaxauur.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2laaauuyk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dlybxcdp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zzergndt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mqsgsyvc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iidcqonc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lrlvezmb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lmnkivav.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mparqyin.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrfljeny.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yrebimtw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fxwvaily.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fcjxvxyb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hjufinuh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2aqnabbqa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2tpulrbyw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2toypslgl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vkxsuymr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gtohdscn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nzlguqyf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rnjrnyqw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ephpmxiv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zxxultve.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kxgbkmpu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cqawutsc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dctrsxqh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kfmxwqxc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2kncqaxbd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tnkfhyai.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kxwozwlg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2adxuxaal.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2iygkbwom.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vwfvozbs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2thzhuygc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lqkvrohu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dodzujru.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2akjdfmzt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rmycfugm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fwguapdf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hzxshnko.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2yigxtwoi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gqqvxxar.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ymbyzprn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tfsukatq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hlfptdrw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gjuyctpe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nglwrccq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2meomrhwr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bxrtjpmx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mwiqmpqa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ndlexoew.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2pmoymhsd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xclqpfpv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2czvwpcwp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ztssomhc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sjefqbfp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ydhqrpwk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ayjzvysj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ovjclrzz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yadcfzzm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2uewwsagn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zkzhjcml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhnftnwo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zudglspc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iciifapd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lfdbluoo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ljtzugiq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mdbenoru.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gemasmph.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zazglddo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2klovjukw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2udpxbpwb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wmrmjusv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rjuysded.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hcjebwfw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2euvszpnd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dmjuoayk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mzkkjmde.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ovahyiju.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2akvwshvi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xnkoxjjg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cavxocit.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2oiplvvsn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2oelwdlkv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hcjbwfkm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jazvdzwl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2upxnhrms.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2uwxyxdqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jtpubonr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tlhsmvgb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymmzcdjc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uprufhrl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2yovvhnlj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gqkvazpw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cnqvouxa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ahzipini.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ipnanfcd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kntkerpb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bhkuoxun.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wjaoajmg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ifbhgsqc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tsetyzmc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rgegczrp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jhemsoni.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2iygofasz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2oikpwveo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2oyjcqfvc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qpeemvqj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ylsmstjq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2frcryecf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2milazuwb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kkzcgszk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qnczifth.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mzgmtgls.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2osjrtizk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2shbcbdho.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bcnzofxy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cyuewpfy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vognlneb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pvyyyghk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xxzxocit.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qzqbudcr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2akcbzyej.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cnmwtfdt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmyrgkzb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xtiweodm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nmyjyoep.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kzjpqzmg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hznbpycl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mbvowkdk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zwkidoip.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2docyhnfh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2hmhgxdjx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yfmofjgi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2bzoixxen.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mnfyiuwp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wjavcqzv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fmrlpmef.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xqhemaks.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gamdzmhc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nbbktdkg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2frabhmso.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qgtzlbub.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2odifxukw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2njjprprg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kejzeqpl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nyjimhji.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ayoxokza.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2eddhfzlg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2aftsxqns.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wowuobqw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbbhprwd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mhzrgzsj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kqojuyct.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gwddpbql.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dnxqsngw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2imgedeun.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dhggujot.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qztdhmrt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zysvehdt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ujbnpjrw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vzwldznx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmadgoiw.html


<!-- 参考信息 -->